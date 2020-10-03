# pacman
# pacman
Câu 1: Tìm kiếm theo chiều sâu:
    B1: Tạo biến lưu các đỉnh đang xét và hàng đợi lưu các đỉnh đang xét, biến lưu các bước đi tự đầu đến nút hiện tại.
    B2: Lấy đỉnh bắt đầu đi. Đánh dấu đã xét đỉnh này và bỏ vào stack.
    B3: Lấy đỉnh đầu trong stack và tìm những đỉnh có kết nối với đỉnh này. Lưu bước đi đến đỉnh được duyệt là từ đỉnh đang xét
    B4: Lặp lại bước 3 đến khi hết stack hoặc xét đến đỉnh cần đến.
    
Câu 2: Tìm kiếm theo chiều rộng
 - Thuật toán tương tự tìm kiếm theo chiều sâu nhưng thay vào đó ta lưu các đỉnh đang xét trong queue

Câu 3: Thay đổi hàm chi phí:
- Thuật toán tương tự tìm kiếm theo chiều rộng nhưng ta sử dụng hàng đợi ưu tiên để lưu các đỉnh đang xét, các đỉnh có chi pjí thấp hơn sẽ được duyệt trước.
- Khi duyệt các nút nếu thấy chi phí thấp hơn chi phí đã có thì gan lại chi phí cho nít này.

Câu 4: Tìm kiếm A*
- Thuật toán giống với Câu 3, chỉ thay điều kiện ưu tiên của hàng đợi ưu tiên theo công thức F = H + G

Câu 5:Tìm tất cả các góc
- Đầu tiên kiểm tra điểm đầu tiên bắt đầu đi có phải ở góc nào không.
- Kiểm tra xem có thể đi đuọc hay không.
- Viết hàm kiếm tra Pacman đã đến đủ 4 gọc hay chưa.
- Tìm kiếm đường đi đến tất cả các góc bằng 1 trong các thuật toán tìm kiếm DFS,BFS,A*

Câu 6: Bài toán góc: Heurític
- Từ điểm khởi đầu, ta liệt kê tất cả quãng đường từ điểm xuất phát cho đến n điểm kết nối với nó rồi chọn đi theo con đường ngắn nhất.
- Khi đã đi đến một điểm kết nối với nó, chọn đi đến điểm kế tiếp cũng theo nguyên tắc trên. Nghĩa là liệt kê tất cả con đường từ điểm bên cạnh ta đang đứng đến những điểm chưa đi đến. Chọn con đường ngắn nhất. 
- Lặp lại quá trình này cho đến lúc không còn đại lý nào để đi.

Câu 7:Ăn hết dấu chấm
- Cho tất cả các cạnh vào hàng đợi ưu tiên.
- Lấy dần ra các cạnh, kiểm tra các cạnh có tạo chu trình hay không, nếu không thì thêm cạnh đó vào 
- Làm đến khi đủ n-1 cạnh ta được đường đi ăn tất cả cấc điểm ngắn nhất

Câu 8: 
- Bắt đầu từ 1 nút, duyệt tất cả các đỉnh liền kề của nút đó, lấy đường đi mà từ nút đng xét đếm nút liền kề có độ dài nhỏ nhất.
- Tiếp tục lấy các nút cho đếm khi đủ tất cả các nút.
