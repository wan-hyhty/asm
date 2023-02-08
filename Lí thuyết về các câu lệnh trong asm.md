# Cú pháp lệnh

Một lệnh asm gồm 4 phần tử sau  
***[Nhãn lệnh:]    <tên lệnh>    [các toán hạng]   [;comment]*** 
  
 Trong đó:  
* ***Nhãn lệnh:*** : Là một dãy các kí tự đứng trước câu lệnh, nó được chỉ định thay thế cho địa chỉ của câu lệnh trong các đoạn lệnh lặp, rẽ nhánh (địa chỉ)  
* ***Tên lệnh*** : Là một trong các lệnh trong tập lệnh (tương tự như printf hay scanf trong nn C). Trong chương trình hợp ngữ mỗi dòng chỉ có thể chứa một lệnh và mỗi lệnh phải được đặt trên một dòng.  
* ***Các toán hạng*** : là đối tượng mà lệnh tác động vào (tạm hiểu là biến). Ở intel 8088/8086 có thể không có toán hạng, có một hoặc 2 toán hạng. Trường hợp có 2 toán hạng thì toán hạng đứng trước là **toán hạng đích** , sau là **toán hạng nguồn** . Nghĩa là lấy toán hạng nguồn thực hiện ***lệnh*** và gán vào toán hạng đích.  
* ***comment*** : là các chú thích tương tự như // của C  
  
Ví dụ:  
mov AX,BX ;đặt giá trị thanh ghi BX vào thanh ghi AX  
* mov: là tên lệnh có chức năng đặt thanh ghi 
* AX: là toán hạng đích  
* BX: là toán hạng nguồn  

# Các lệnh cơ bản 
## Mov (move)  
*có thể hiểu là phép gán*  
***MOV [toán hạng đích] , [toán hạng nguồn]***  
* **toán hạng đích** : có thể là thanh ghi (8bit or 16bit), địa chỉ của một ô nhớ, một biến nào đó và không thể là hằng số.  
* **toán hạng nguồn** : có thể là hằng số, biến, thanh ghi, địa chỉ của một ô nhớ.  
  
*Lưu ý*  
mov AX, DI   ;đặt thanh ghi DI vào thanh ghi AX (địa chỉ thanh ghi)
mov AX, [DI] ;nội dung của ô nhớ được chỉ bởi DI Tức là, đặt nội dung của ô nhớ được chỉ bởi DI vào thanh ghi Ax: Ax = 41h  

