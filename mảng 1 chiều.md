1. Khái niệm

Mảng 1 chiều là một tập hợp nhiều phần tử cùng kiểu dữ liệu, được lưu liên tiếp trong bộ nhớ.

Truy cập phần tử bằng chỉ số (index), bắt đầu từ 0.

2. Cú pháp khai báo
kieu_du_lieu ten_mang[so_phan_tu];


Ví dụ:

int a[5];   // mảng a có 5 phần tử kiểu int (chỉ số: 0 → 4)

3. Khởi tạo mảng

Có nhiều cách:

int a[5] = {1, 2, 3, 4, 5};       // khởi tạo đầy đủ
int b[5] = {1, 2};                // còn lại tự động = 0 → {1,2,0,0,0}
int c[]  = {10, 20, 30};          // compiler tự hiểu kích thước là 3

4. Truy cập phần tử

Cú pháp:

ten_mang[index]


a[0] → phần tử đầu tiên

a[4] → phần tử cuối cùng (nếu mảng có 5 phần tử)

5. Nhập và xuất mảng

Ví dụ nhập mảng 5 số và in ra:

#include <stdio.h>

int main() {
    int a[5];
    
    // Nhập
    for(int i = 0; i < 5; i++) {
        printf("Nhap a[%d]: ", i);
        scanf("%d", &a[i]);
    }

    // Xuất
    printf("Mang vua nhap: ");
    for(int i = 0; i < 5; i++) {
        printf("%d ", a[i]);
    }

    return 0;
}
