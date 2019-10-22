# multiagent
Câu 1:
  Hàm evaluationFunction trả về giá trị value, 
  value = (điểm đã có - 10.0/(khoảng cách mahatan từ pacman đến ghost) + 10.0/(khoảng cách mahattan từ pacman đến thức ăn gần nhất))
Câu 2:
  1) Kiểm tra nếu là ghost cuối cùng thì
    - Nếu là max depth thì trả về điểm số của trạng thái trò chơi thông qua hàm evaluationFunction
    - Ngược lại thì duyệt tiếp với pacman với depth+1
  2) Nếu ko phải là ghost cuối
    - lấy danh sách các hành động có thể thực hiện của agent tương ứng
    - nếu danh sách vừa lấy rỗng thì trả về điểm của trạng thái trò chơi
    - lấy danh sách điểm khi cho agent thực hiện hành trong danh sách hành động có thể thực hiện
    - nếu là pacman thì trả về max của danh sách điểm
    - nếu là ghost thì trả về min của danh sách điểm
  3) Hàm action trả về hành động tương ứng với điểm lớn nhất của pacman
Câu 3:
  - Hàm getMaxValue trả về giá trị lớn nhất tốt nhất và hành động tương ứng
  - Hàm getMinValue trả về giá trị nhỏ nhất tốt nhất và hành động tương ứng
Câu 4:
  Tương tự như câu 2, nhưng thay vì trả về min cho ghost ta trả về giá trị trung bình
