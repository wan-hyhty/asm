# Cú pháp lệnh

Một lệnh asm gồm 4 phần tử sau  
***[Nhãn lệnh:]    <tên lệnh>    [các toán hạng]   [;comment]*** 
  
  Trong đó:  
  \***Nhãn lệnh:\*** : Là một dãy các kí tự đứng trước câu lệnh, nó được chỉ định thay thế cho địa chỉ của câu lệnh trong các đoạn lệnh lặp, rẽ nhánh (địa chỉ)  
  \***Tên lệnh\*** : Là một trong các lệnh trong tập lệnh (tương tự như printf hay scanf trong nn C). Trong chương trình hợp ngữ mỗi dòng chỉ có thể chứa một lệnh và mỗi lệnh phải được đặt trên một dòng.  
  \***Các toán hạng\*** : là đối tượng mà lệnh tác động vào (tạm hiểu là biến). Ở intel 8088/8086 có thể không có toán hạng, có một hoặc 2 toán hạng. Trường hợp có 2 toán hạng thì toán hạng đứng trước là \**toán hạng đích\** , sau là \**toán hạng nguồn\** . Nghĩa là lấy toán hạng nguồn thực hiện ***lệnh*** và gán vào toán hạng đích.

