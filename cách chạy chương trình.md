# Biên soạn và liên kết một chương trình lắp ráp trong NASM
Nhập đoạn mã trên bằng trình soạn thảo văn bản và lưu nó dưới dạng tên.asm  
Đảm bảo rằng bạn đang ở trong cùng một thư mục với nơi bạn đã lưu tên.asm.  
Để complie **nasm -f elf tên.asm**  
Nếu có bất kỳ lỗi nào, bạn sẽ được nhắc về điều đó ở giai đoạn này. Nếu không, một tệp đối tượng của chương trình của bạn có tên tên.o sẽ được tạo  
Để liên kết tệp đối tượng và tạo một tệp thực thi có tên hello, hãy nhập ld -m elf_i386 -s -o hello hello.o  
Thực thi chương trình bằng cách gõ ./hello  
