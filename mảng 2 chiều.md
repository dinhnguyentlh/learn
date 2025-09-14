1. Khái niệm

Mảng 1 chiều: lưu trữ nhiều phần tử cùng kiểu dữ liệu, nằm liên tiếp trong bộ nhớ.

int a[5] = {1,2,3,4,5};


Mảng 2 chiều: thực chất là một mảng của mảng 1 chiều → dùng để biểu diễn dạng bảng (hàng, cột).

int a[3][4]; // mảng 2 chiều có 3 hàng, 4 cột

2. Khai báo mảng 2 chiều
type arrayName[soHang][soCot];


Ví dụ:

int a[2][3]; // 2 hàng, 3 cột

3. Khởi tạo giá trị
int a[2][3] = {
    {1,2,3},
    {4,5,6}
};


Hoặc viết gọn:

int a[2][3] = {1,2,3,4,5,6};

4. Truy cập phần tử

Cú pháp:

a[hang][cot]


a[0][0] → phần tử hàng 0, cột 0

a[1][2] → phần tử hàng 1, cột 2

5. Duyệt mảng 2 chiều (for lồng nhau)
#include <stdio.h>

int main() {
    int a[2][3] = {{1,2,3},{4,5,6}};
    for(int i = 0; i < 2; i++) {        // duyệt hàng
        for(int j = 0; j < 3; j++) {    // duyệt cột
            printf("%d ", a[i][j]);
        }
        printf("\n");
    }
    return 0;
}


👉 Output:

1 2 3
4 5 6
