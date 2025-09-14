1. Khái niệm

Hàm là một khối lệnh được đặt tên, dùng để thực hiện một nhiệm vụ cụ thể.

Giúp chia chương trình thành các phần nhỏ, dễ quản lý, tái sử dụng.

2. Cấu trúc khai báo hàm
kieu_tra_ve ten_ham(kieu_tham_so1 tham_so1, kieu_tham_so2 tham_so2, ...) {
    // phần thân hàm: các câu lệnh
    return gia_tri; // nếu có kiểu trả về
}

3. Ví dụ hàm không trả về, không có tham số
#include <stdio.h>

void xinChao() {
    printf("Hello, xin chao ban!\n");
}

int main() {
    xinChao();  // gọi hàm
    return 0;
}

4. Hàm có tham số, có trả về
#include <stdio.h>

// hàm cộng 2 số nguyên
int cong(int a, int b) {
    return a + b;
}

int main() {
    int x = 5, y = 7;
    int kq = cong(x, y); // gọi hàm
    printf("Tong = %d\n", kq);
    return 0;
}


👉 Output:

Tong = 12

5. Phân loại hàm

Hàm có sẵn: do thư viện C cung cấp

printf, scanf, sqrt, strlen, …

Hàm tự định nghĩa: do người lập trình viết

6. Quy tắc đặt hàm

Tên hàm phải bắt đầu bằng chữ cái hoặc _, không được chứa dấu cách.

Nên đặt tên gợi nhớ chức năng (tinhTong, max, nhapMang, …).
