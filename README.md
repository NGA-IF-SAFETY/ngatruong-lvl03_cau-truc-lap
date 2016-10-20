A)Cấu trúc lặp for

1.Cú pháp: 

            for (biểu thức 1; biểu thức 2; biểu thức 3)            Khối lệnh; 

Trong đó: 
    Biểu thức 1: biểu thức khởi đầu.

    Biểu thức 2: biểu thức điều kiện - điều kiện lặp.

    Biểu thức 3: bước nhảy - thường dùng với ý nghĩa là thay đổi bước nhảy.

Cả 3 biểu thức này đều là tuỳ chọn, chúng có thể vắng mặt trong câu lệnh cụ thể nhưng các dấu chấm phẩy vẫn phải có.

Sự hoạt động của vòng lặp for: 

  • Bước 1: Thực hiện biểu thức khởi đầu – Biểu thức 1.

 
  • Bước 2: Tính giá trị biểu thức 2 để xác định điều kiện lặp.

          Nếu biểu thức 2 có giá trị ‘sai’ (==0) thì ra khỏi vòng lặp.

          Ngược lại, nếu biểu thức có giá trị ‘đúng’ ( khác 0) thì chuyển tới bước 3.

   • Bước 3: Thực hiện khối lệnh sau for ( thân của for ), chuyển tới bước 4.
   
   • Bước 4: Thực hiện biểu thức 3, rồi quay về bước 2.

 * SƠ ĐỒ KHỐI

   ![ ](http://1.bp.blogspot.com/-ognNzsULg8E/TgYeKlQenLI/AAAAAAAAABY/AVGrzmQ9B0M/s1600/1.bmp)

   2.VÍ DỤ 

   #include<stdio.h>   

   #include<conio.h>

   void main()

{

 int n,i;

float s=0;

printf("nhap vao n so dau tien : \n");

scanf("%d",&n);

for(i=1;i<=n;i++)

s=s+(float)1/i ;

printf("tong n so dau tien cua day so:0.2%f",s);

}

B)CẤU TRÚC LẶP DO... WHILE

1.Cú pháp:

               do

               Khối lệnh; 

               while (biểu thức); 

Giải thích cú pháp: 

Bước 1: thực hiện khối lệnh sau do.

Bước 2: kiểm tra giá trị biểu thức <biểu thức> sau while, nếu có giá trị ‘đúng’ ( khác 0) thì lặp lại bước 1, nếu ‘sai’ (=0) thì kết thúc vòng lặp.

SƠ ĐỒ KHỐI

![ ] (http://4.bp.blogspot.com/-T1XhDnpgUZU/TgYdCIm76xI/AAAAAAAAABU/QTJmQLCb6Ko/s1600/1.bmp)

2.Ví dụ:

#include <stdio.h> 


 # define PASSWORD 

 void main(void) 

 {  

   int in; 

   do  

  {  

    printf("Nhap vao password: "); 

    scanf("%d", &in);

   }

   while (in != PASSWORD); 

 } 

 C)CẤU TRÚC LẶP while

 1. Cú pháp:

            while(biểu thức)

            Khối lệnh;   


Sự hoạt động của vòng lặp while:

Bước 1: tính giá trị của (biểu thức) sau while

Bước 2: nếu giá trị tính được của (biểu thức) là ‘sai’ (==0) thì kết thúc  vòng lặp while. 

Bước 3: nếu giá trị của (biểu thức) là ‘đúng’ (!=0) thì thực hiện khối lệnh sau while.

Bước 4: quay lại bước 1

  SƠ ĐỒ KHỐI

  ![ ](http://icviet.vn/upload/images/lap%20trinh%20c%20co%20ban/Bai%206/1.PNG)

    2.ví dụ 

 #include <stdio.h> 

#include <conio.h> 

void main()

{

  int i = 0, in, is = 0; 

  printf("Nhap vao so n: ");

  scanf("%d", &in);  

  while (i++ < in) 

  is = is + i;   

  printf("Tong: %d", is); 

  getch();

} 
