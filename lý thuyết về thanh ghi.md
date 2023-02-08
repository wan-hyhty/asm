Có 10 thanh ghi 32-bit và 6 thanh ghi 16-bit. Được chia thành 3 nhóm sau:  
* thanh ghi chung (general register)  
* thanh ghi điều kiển (control register)  
* thanh ghi Segment (Segment register)  
trong thanh ghi general được chia thành 3 nhóm sau:  
* thanh ghi data
* thanh ghi con trỏ (pointer)
* thanh ghi index (chỉ số)  
1. **thanh ghi data (registers)**  
có 4 thanh ghi data 32bit được sử dụng cho số học, logic và các hoạt dộng khác. Các thanh ghi 32 được sử dung theo 3 cách sau:  
* là thanh ghi data 32bit: EAX, EBX, ECX, EDX.  
* nửa thanh ghi cảu 32 bit có thể được sử dụng làm 4 thanh ghi data 16bit: AX, BX,CX,DX  
* trong thanh ghi 16bit chia nửa thành 8 thanh ghi dữ liệu 8 bit AH, AL, BH, BL,CH, CL,DH, CL  
![image](https://user-images.githubusercontent.com/111769169/217571710-f9c040bb-e8ca-447b-964f-3b9b8383cf27.png)  
* AX là primary accumulator, được sử dụng trong đầu vào / ra và hầu hết các hướng dẫn số học. ví dụ, trong phép nhân, một toán hạng được lưu trong thanh ghi EAX hoặc AX AL theo kích thước của toán hạng. BX được gọi là base register  
* BX được biết là base register (thanh ghi cơ sở), vì nó được sử dụng trong indexed addressing.  
* CX được gọi là count register, vì thanh ECX, CX lưu trữ số vòng lặp trong các phép táon lặp ( tương tự việc khai báo biến i và tăng biến i để tạo thành vòng lặp trong c)  
* DX: thanh ghi dữ liệu, được sử dụng để setup đầu vào đầu ra. Được sử dụng với thanh AX cùng DX để nhân và chia các hoạt động liên quan đến các giá trị lớn
