# Week 8: FUNCTIONAL REQUIREMENT SPECIFICATIONS
# Thành viên:
* Trần Ngọc Lâm (5*)
* Kiều Duy Nam (5*)
* Nông Ngọc Huân (5*)
* Mai Phúc Lâm (5*)
* Dương Đức Bình (5*)
* Đoàn Hữu Bách (5*)
# Week 8: FUNCTIONAL REQUIREMENT SPECIFICATIONS
# Thành viên:
* Trần Ngọc Lâm (5*)
* Kiều Duy Nam (5*)
* Nông Ngọc Huân (5*)
* Mai Phúc Lâm (5*)
* Dương Đức Bình (5*)
* Đoàn Hữu Bách (5*)
# I System of requirements
| Identifier | Priority Weight | Requirements | 
| :----- | :---------- | :-------------- | 
| REQ-1 | 10 | hệ thống có phần đăng nhập và đăng kí| 
| REQ-2 | 8 | hệ thống có chức năng chỉnh sửa thông tin sản phẩm | 
| REQ-3 | 5|  hệ thống có chức năng thêm sản phẩm | 
| REQ-4| 5|  hệ thống có chức năng xóa sản phẩm               |
| REQ-5| 3|  hệ thống có chức năng tìm kiếm sản phẩm              |
| REQ-6| 3|  hệ thống có chức năng sắp xếp sản phẩm               |
| REQ-7| 10|  hệ thống có chức năng thống kê doanh thu  |
| REQ-8| 5|  hệ thống có chức năng xem hàng tồn              |
| REQ-9| 7|  hệ thống có chức năng thống kê hạn sử dụng   |
| REQ-10| 5|  hệ thống có chức năng xuất hóa đơn cho khách hàng|
| REQ-11| 10|  hệ thống có chức năng xuất hóa đơn cuối ca     |
| REQ-12| 10|  hệ thống có chức năng xuất kiểm tra lịch sử bán hàng     |
| REQ-13| 10|  hệ thống có chức năng đăng xuất và xóa tài khoản            |
| REQ-14| 10|  hệ thống có chức năng thanh toán nhiều hình thức            |
| REQ-15| 3|  hệ thống có chức năng báo lỗi cho quản trị viên    |


| Actor | Actor's Goal | Use Case Name | 
| :----- | :---------- | :-------------- | 
| Visitor/User/Admin | Để đăng nhập vào ứng dụng |Login (UC-1) | 
| Visitor/User/Admin | Để đăng ký vào hệ thống ứng dụng | Register (UC-2) | 
| Visitor/User/Admin | Để xóa tài khoản | Register (UC-2) |
| Visitor/User | Để chỉnh sửa thông tin sản phẩm | Update(UC-3)  | 
| Visitor/User | Để thêm sản phẩm           | Add(UC-4)    |
| Visitor/User | Để chỉnh xóa sản phẩm | Delete(UC-5)  | 
| Visitor/User | Để chỉnh sửa thông tin sản phẩm | Update(UC-6)  | 
| Visitor/User | Để sắp xếp sản phẩm | QLK(UC-7)  | 
| Visitor/User | Để xem hàng tồn| QLK(UC-7)  | 
| Visitor/User | Để thống kê hsd| QLK(UC-7)  |
| Visitor/User | Để tìm kiếm sản phẩm | QLK(UC-7)  |
| Visitor/User | Để xuất hóa đơn cho khách hàng  | SaoKe(UC-8)  | 
| Visitor/User | Để xuất hóa đơn cuối ca | SaoKe(UC-8)  | 
| User | Để thông kê doanh thu | SaoKe(UC-8)  |
| Visitor/User | Để xuất hóa đơn cho khách hàng| ThanhToan(UC-9)  | 
| Visitor/User | Để thanh toán nhiều hình thức | ThanhToan(UC-9)  |
| User | Để báo lỗi cho QTV | Erorr(UC-10)  |
| DataBase/Repository | Để lưu trữ dữ liệu, phân quyền người dùng, lịch sử giao dịch | UC-1,UC-2,UC-3,UC-4,UC-5,UC-6,UC-7,UC-8,UC-9  | 

#  III. Use Cases
## i. Casual Description
# REQ – 1 : hệ thống có phần đăng nhập và đăng kí 
Mô tả chung:
Người dùng muốn truy cập vào hệ thống cần phải có tài khoản. Hệ thống cung cấp hai chức năng cho người dùng đăng ký tài khoản mới hoặc đăng nhập vào tài khoản đã có.

Các bước thực hiện:

Đăng ký tài khoản mới:
-	Người dùng chọn chức năng "Đăng ký".
-	Hệ thống hiển thị giao diện đăng ký, yêu cầu người dùng nhập thông tin cá nhân bao gồm: họ và tên, địa chỉ email, số điện thoại, tên đăng nhập và mật khẩu.
-	Người dùng nhập thông tin và gửi yêu cầu đăng ký tài khoản.
-	Hệ thống kiểm tra thông tin người dùng nhập và tạo tài khoản mới cho người dùng.
-	Hệ thống hiển thị thông báo đăng ký thành công và yêu cầu người dùng đăng nhập để truy cập vào hệ thống.
Đăng nhập vào tài khoản đã có:
-	Người dùng chọn chức năng "Đăng nhập".
-	Hệ thống hiển thị giao diện đăng nhập, yêu cầu người dùng nhập tên đăng nhập và mật khẩu đã đăng ký trước đó.
-	Người dùng nhập thông tin tài khoản và gửi yêu cầu đăng nhập.
-	Hệ thống kiểm tra thông tin tài khoản và xác thực người dùng.
-	Nếu thông tin tài khoản hợp lệ, hệ thống cho phép người dùng truy cập vào hệ thống và hiển thị giao diện chính của ứng dụng.
-	Nếu thông tin tài khoản không hợp lệ, hệ thống hiển thị thông báo lỗi và yêu cầu người dùng nhập lại thông tin tài khoản.
Điều kiện tiên quyết:

Hệ thống đã được cài đặt và có kết nối internet để truy cập vào hệ thống.
Kết quả:

Người dùng có thể đăng ký tài khoản mới hoặc đăng nhập vào tài khoản đã có để truy cập vào hệ thống.
Hệ thống có thể xác thực người dùng và hiển thị giao diện chính của ứng dụng nếu thông tin tài khoản hợp lệ.
# REQ-2 : hệ thống có chức năng chỉnh sửa thông tin sản phẩm
Mô tả chung:
Người dùng muốn chỉnh sửa thông tin của một sản phẩm trong hệ thống. Hệ thống cung cấp chức năng cho người dùng thực hiện chỉnh sửa thông tin sản phẩm đó.

Các bước thực hiện:

-	Chỉnh sửa thông tin sản phẩm:
-	Người dùng chọn sản phẩm cần chỉnh sửa từ danh sách sản phẩm hiển thị trên giao diện.
-	Hệ thống hiển thị thông tin chi tiết của sản phẩm, bao gồm tên sản phẩm, mô tả, giá, số lượng, hình ảnh, và các thông tin khác liên quan đến sản phẩm.
-	Người dùng thực hiện chỉnh sửa thông tin cần thiết trên giao diện chỉnh sửa, bao gồm: tên sản phẩm, mô tả, giá, số lượng, hình ảnh và các thông tin khác liên quan đến sản phẩm.
-	Người dùng lưu lại các thông tin chỉnh sửa bằng cách bấm nút "Lưu".
-	Hệ thống kiểm tra các thông tin chỉnh sửa và cập nhật vào cơ sở dữ liệu.
-	Hệ thống hiển thị thông báo chỉnh sửa thành công và hiển thị lại thông tin chi tiết sản phẩm đã được chỉnh sửa.
Điều kiện tiên quyết:
-	Người dùng đã đăng nhập vào hệ thống và có quyền truy cập vào danh sách sản phẩm.
-	Sản phẩm cần chỉnh sửa đã được tạo trước đó và có trong cơ sở dữ liệu của hệ thống.
Kết quả:
-	Người dùng có thể chỉnh sửa thông tin của một sản phẩm trong hệ thống.
-	Hệ thống có thể kiểm tra và cập nhật các thông tin chỉnh sửa vào cơ sở dữ liệu.
-	Người dùng có thể xem lại thông tin chi tiết của sản phẩm sau khi chỉnh sửa.

# REQ-3 : hệ thống có chức năng thêm sản phẩm
Mô tả chung:
Người dùng muốn thêm một sản phẩm mới vào hệ thống. Hệ thống cung cấp chức năng cho người dùng thêm sản phẩm mới.

Các bước thực hiện:

Thêm sản phẩm mới:
-	Người dùng chọn chức năng "Thêm sản phẩm" trên giao diện hệ thống.
-	Hệ thống hiển thị một giao diện để người dùng nhập thông tin sản phẩm mới, bao gồm: tên sản phẩm, mô tả, giá, số lượng, hình ảnh và các thông tin khác liên quan đến sản phẩm.
-	Người dùng nhập thông tin sản phẩm mới và bấm nút "Thêm sản phẩm".
-	Hệ thống kiểm tra thông tin sản phẩm và lưu vào cơ sở dữ liệu.
-	Hệ thống hiển thị thông báo thêm sản phẩm thành công và hiển thị lại danh sách các sản phẩm trong hệ thống.
Điều kiện tiên quyết:

-	Người dùng đã đăng nhập vào hệ thống và có quyền thêm sản phẩm mới.
-	Các thông tin sản phẩm mới nhập vào phải hợp lệ và chưa có trong cơ sở dữ liệu của hệ thống.
Kết quả:

Người dùng có thể thêm sản phẩm mới vào hệ thống.
Hệ thống có thể kiểm tra và lưu thông tin sản phẩm mới vào cơ sở dữ liệu.
Người dùng có thể xem danh sách sản phẩm mới bao gồm sản phẩm vừa được thêm vào.
# REQ-4: hệ thống có chức năng xóa sản phẩm

Mô tả chung:
Người dùng muốn xóa một sản phẩm khỏi hệ thống. Hệ thống cung cấp chức năng cho người dùng xóa sản phẩm.

Các bước thực hiện:

Xóa sản phẩm:
-	Người dùng chọn sản phẩm cần xóa trên giao diện hệ thống.
-	Người dùng chọn chức năng "Xóa sản phẩm".
-	Hệ thống hiển thị thông báo xác nhận xóa sản phẩm, hỏi người dùng có chắc chắn muốn xóa sản phẩm hay không.
-	Nếu người dùng chọn "Có", hệ thống xóa sản phẩm khỏi cơ sở dữ liệu và hiển thị thông báo xóa sản phẩm thành công.
-	Nếu người dùng chọn "Không", hệ thống không thực hiện xóa sản phẩm và quay lại trang trước đó.
Điều kiện tiên quyết:

Người dùng đã đăng nhập vào hệ thống và có quyền xóa sản phẩm.
Sản phẩm cần xóa phải tồn tại trong cơ sở dữ liệu của hệ thống.
Kết quả:

Người dùng có thể xóa sản phẩm khỏi hệ thống.
Hệ thống có thể kiểm tra và xóa thông tin sản phẩm khỏi cơ sở dữ liệu.
Người dùng có thể xem lại danh sách các sản phẩm còn lại trong hệ thống.

# REQ-5: hệ thống có chức năng tìm kiếm sản phẩm 
Mô tả chung:
Người dùng muốn tìm kiếm sản phẩm trong hệ thống. Hệ thống cung cấp chức năng cho người dùng tìm kiếm sản phẩm theo tên, giá hoặc mô tả.

Các bước thực hiện:

Tìm kiếm sản phẩm:
-	Người dùng nhập từ khóa tìm kiếm vào ô tìm kiếm trên giao diện hệ thống.
-	Người dùng chọn tiêu chí tìm kiếm là tên, giá hoặc mô tả.
-	Hệ thống hiển thị danh sách các sản phẩm phù hợp với từ khóa tìm kiếm và tiêu chí tìm kiếm được chọn.
-	Người dùng có thể chọn một sản phẩm trong danh sách để xem thông tin chi tiết của sản phẩm.
Điều kiện tiên quyết:

-	Hệ thống có thông tin sản phẩm và các thông tin liên quan được lưu trong cơ sở dữ liệu.
-	Người dùng đã đăng nhập vào hệ thống.
Kết quả:

Người dùng có thể tìm kiếm sản phẩm theo tên, giá hoặc mô tả.
Hệ thống hiển thị danh sách các sản phẩm phù hợp với từ khóa tìm kiếm và tiêu chí tìm kiếm được chọn.
Người dùng có thể xem thông tin chi tiết của sản phẩm.	

# REQ-6: hệ thống có chức năng sắp xếp sản phẩm

Mô tả chung:
Người dùng muốn sắp xếp các sản phẩm theo thứ tự tăng dần hoặc giảm dần của giá, tên hoặc danh mục.

Các bước thực hiện:

Sắp xếp sản phẩm:
-	Người dùng chọn tiêu chí sắp xếp là giá, tên hoặc danh mục.
-	Người dùng chọn thứ tự sắp xếp là tăng dần hoặc giảm dần.
-	Hệ thống sắp xếp danh sách sản phẩm theo tiêu chí và thứ tự được chọn và hiển thị kết quả cho người dùng.
Điều kiện tiên quyết:

-	Hệ thống có thông tin sản phẩm và các thông tin liên quan được lưu trong cơ sở dữ liệu.
-	Người dùng đã đăng nhập vào hệ thống.
Kết quả:

Người dùng có thể sắp xếp các sản phẩm theo thứ tự tăng dần hoặc giảm dần của giá, tên hoặc danh mục.
Hệ thống hiển thị danh sách các sản phẩm được sắp xếp theo tiêu chí và thứ tự được chọn.
# REQ-7: hệ thống có chức năng thống kê doanh thu

Mô tả chung:
Người quản lý muốn thống kê doanh thu của cửa hàng hoặc của một thời gian cụ thể để đưa ra quyết định kinh doanh.

Các bước thực hiện:

Chọn tiêu chí thống kê:
-	Người dùng chọn tiêu chí thống kê doanh thu, ví dụ như doanh thu theo ngày, tháng, năm, sản phẩm, danh mục sản phẩm, khách hàng hoặc nhân viên.
Chọn thời gian thống kê:
-	Người dùng chọn thời gian để thống kê, ví dụ như thống kê doanh thu trong tháng 3 năm 2022.
Hệ thống thực hiện thống kê:
-	Hệ thống truy vấn cơ sở dữ liệu và tính toán doanh thu dựa trên tiêu chí và thời gian được chọn.
-	Hệ thống hiển thị kết quả thống kê cho người dùng dưới dạng bảng hoặc biểu đồ, bao gồm tổng doanh thu, số lượng sản phẩm đã bán, số lượng khách hàng, số lượng nhân viên, chi phí và lợi nhuận.
Điều kiện tiên quyết:

Hệ thống phải có dữ liệu doanh thu, sản phẩm, danh mục sản phẩm, khách hàng, nhân viên và chi phí được lưu trữ trong cơ sở dữ liệu.
Người dùng có quyền truy cập vào các thông tin này.
Kết quả:

Người dùng có thể thống kê doanh thu theo nhiều tiêu chí khác nhau và thời gian cụ thể.
Hệ thống hiển thị kết quả thống kê cho người dùng dưới dạng bảng hoặc biểu đồ để giúp người dùng dễ dàng hiểu và đưa ra quyết định kinh doanh chính xác.

# REQ-8: hệ thống có chức năng xem hàng tồn
Mô tả chung:
Người quản lý muốn xem số lượng hàng tồn trong kho để quản lý và đưa ra quyết định kinh doanh.

Các bước thực hiện:

Mở chức năng xem hàng tồn:
-	Người dùng chọn chức năng xem hàng tồn trong hệ thống quản lý kho.
Chọn kho cần xem:
-	Người dùng chọn kho cần xem hàng tồn.
Hệ thống thực hiện xem hàng tồn:
-	Hệ thống truy vấn cơ sở dữ liệu và tính toán số lượng hàng tồn dựa trên thông tin trong kho được chọn.
-	Hệ thống hiển thị số lượng hàng tồn của mỗi sản phẩm trong kho được chọn.
Tùy chọn chức năng khác:
Người dùng có thể thực hiện các chức năng khác như xem thông tin sản phẩm, chỉnh sửa số lượng hàng tồn, tạo đơn hàng nhập kho để cập nhật số lượng hàng tồn, v.v.
Điều kiện tiên quyết:

Hệ thống phải có dữ liệu số lượng hàng tồn của mỗi sản phẩm được lưu trữ trong cơ sở dữ liệu.
Người dùng có quyền truy cập vào các thông tin này.
Kết quả:

Người dùng có thể xem số lượng hàng tồn của mỗi sản phẩm trong kho.
Hệ thống hiển thị thông tin hàng tồn theo cách dễ dàng hiểu để giúp người dùng quản lý hàng tồn và đưa ra quyết định kinh doanh chính xác.

# REQ-9: hệ thống có chức năng thống kê hạn sử dụng
Mô tả chung:
Người quản lý muốn xem thông tin hạn sử dụng của sản phẩm để quản lý và đưa ra quyết định kinh doanh.

Các bước thực hiện:

Mở chức năng thống kê hạn sử dụng:
-	Người dùng chọn chức năng thống kê hạn sử dụng trong hệ thống quản lý kho.
Chọn kho cần thống kê:
-	Người dùng chọn kho cần thống kê hạn sử dụng sản phẩm.
Hệ thống thực hiện thống kê hạn sử dụng:
-	Hệ thống truy vấn cơ sở dữ liệu và tính toán hạn sử dụng dựa trên thông tin trong kho được chọn.
-	Hệ thống hiển thị danh sách các sản phẩm còn hạn sử dụng theo thời gian còn lại của từng sản phẩm.
Tùy chọn chức năng khác:
-	Người dùng có thể thực hiện các chức năng khác như xem thông tin sản phẩm, chỉnh sửa thông tin sản phẩm, v.v.
Điều kiện tiên quyết:

Hệ thống phải có dữ liệu hạn sử dụng của sản phẩm được lưu trữ trong cơ sở dữ liệu.
Người dùng có quyền truy cập vào các thông tin này.
Kết quả:

Người dùng có thể xem thông tin hạn sử dụng của từng sản phẩm trong kho.
Hệ thống hiển thị thông tin hạn sử dụng theo cách dễ dàng hiểu để giúp người dùng quản lý sản phẩm và đưa ra quyết định kinh doanh chính xác.
# REQ-10: hệ thống có chức năng xuất hóa đơn cho khách hàng
Mô tả chung:
Sau khi khách hàng đã thanh toán, người quản lý muốn xuất hóa đơn cho khách hàng để cung cấp thông tin chi tiết về đơn hàng.

Các bước thực hiện:

Mở chức năng xuất hóa đơn:
-	Người dùng chọn chức năng xuất hóa đơn trong hệ thống quản lý bán hàng.
Tìm kiếm đơn hàng:
-	Người dùng tìm kiếm đơn hàng cần xuất hóa đơn bằng cách nhập thông tin đơn hàng hoặc chọn đơn hàng từ danh sách đơn hàng trong hệ thống.
Xác nhận thông tin đơn hàng:
-	Hệ thống hiển thị thông tin chi tiết về đơn hàng và xác nhận các thông tin về số lượng, giá cả, v.v.
Xuất hóa đơn:
-	Người dùng chọn chức năng xuất hóa đơn.
-	Hệ thống tạo hóa đơn chứa thông tin chi tiết về đơn hàng, bao gồm thông tin sản phẩm, số lượng, giá cả, tổng giá trị đơn hàng, thông tin khách hàng, v.v.
-	Hệ thống hiển thị hóa đơn để người dùng có thể in ra hoặc lưu trữ vào hệ thống.
Điều kiện tiên quyết:

Đơn hàng của khách hàng phải đã được thanh toán trước đó.
Hệ thống phải có thông tin chi tiết đơn hàng và thông tin khách hàng được lưu trữ trong cơ sở dữ liệu.
Kết quả:

Người dùng có thể xuất hóa đơn cho khách hàng dễ dàng và nhanh chóng.
Hóa đơn chứa thông tin chi tiết về đơn hàng, giúp khách hàng và người quản lý có thể kiểm tra các thông tin đơn hàng một cách chính xác.

# REQ-11: hệ thống có chức năng xuất hóa đơn cuối ca
Mô tả chung:
Hệ thống có chức năng xuất hóa đơn cuối ca, cho phép người quản lý có thể in ra bản hóa đơn tổng hợp của toàn bộ các đơn hàng được ghi nhận trong một ca làm việc.

Các bước thực hiện:

-	Người quản lý truy cập vào hệ thống và chọn chức năng "Xuất hóa đơn cuối ca".
-	Hệ thống sẽ truy vấn tất cả các đơn hàng được ghi nhận trong ca làm việc hiện tại.
-	Hệ thống sẽ tổng hợp thông tin của các đơn hàng này, bao gồm thông tin sản phẩm, số lượng, giá cả và tổng tiền.
-	Người quản lý có thể kiểm tra và chỉnh sửa thông tin của hóa đơn tổng hợp nếu cần thiết.
-	Người quản lý in hoặc xuất file PDF của hóa đơn tổng hợp để sử dụng.
Điều kiện tiên quyết:

Người quản lý đã đăng nhập vào hệ thống và có quyền truy cập chức năng "Xuất hóa đơn cuối ca".
Hệ thống phải ghi nhận được các đơn hàng được thực hiện trong ca làm việc hiện tại.
Kết quả:

Người quản lý có thể in ra bản hóa đơn tổng hợp của toàn bộ các đơn hàng được ghi nhận trong một ca làm việc.
Hóa đơn tổng hợp cung cấp thông tin chi tiết về các sản phẩm bán ra, số lượng, giá cả và tổng tiền, giúp người quản lý kiểm tra và theo dõi doanh thu của cửa hàng.

# REQ-12: hệ thống có chức năng xuất kiểm tra lịch sử bán hàng

Mô tả: Use case này mô tả chức năng của hệ thống để xuất báo cáo lịch sử bán hàng.

Người tham gia: Quản lý, Quản trị viên

Điều kiện tiên quyết: Hệ thống phải đã ghi lại tất cả các giao dịch bán hàng.

Các bước thực hiện:

-	Quản lý hoặc Quản trị viên đăng nhập vào hệ thống.
-	Quản lý hoặc Quản trị viên chọn chức năng "Xuất báo cáo lịch sử bán hàng".
-	Hệ thống hiển thị một biểu mẫu để chọn phạm vi ngày cho báo cáo.
-	Quản lý hoặc Quản trị viên chọn phạm vi ngày cho báo cáo.
-	Hệ thống tạo một báo cáo chứa thông tin sau đây:
Ngày và giờ bán hàng
ID của bán hàng
Các sản phẩm đã bán và số lượng của chúng
Tổng giá trị bán hàng
Hệ thống xuất báo cáo sang tệp CSV hoặc Excel.
Luồng thay thế: Nếu không có giao dịch bán hàng trong phạm vi ngày được chọn, hệ thống hiển thị một thông báo cho biết không có dữ liệu để xuất.

Điều kiện kết thúc: Quản lý hoặc Quản trị viên nhận được báo cáo lịch sử bán hàng trong tệp CSV hoặc Excel. Báo cáo có thể được sử dụng cho mục đích phân tích và lưu trữ.
# REQ-13: hệ thống có chức năng đăng xuất và xóa tài khoản
Mô tả chung:

Use case "Đăng xuất và xóa tài khoản" miêu tả chức năng cho phép người dùng đăng xuất khỏi hệ thống và xóa tài khoản của mình.

Các bước thực hiện:

-	Người dùng truy cập vào phần "Đăng xuất" hoặc "Xóa tài khoản" trong giao diện người dùng.
-	Nếu người dùng chọn "Đăng xuất", hệ thống sẽ xác nhận và đăng xuất người dùng khỏi hệ thống.
-	Nếu người dùng chọn "Xóa tài khoản", hệ thống sẽ hiển thị cảnh báo và yêu cầu xác nhận việc xóa tài khoản.
-	Sau khi xác nhận, hệ thống sẽ xóa tài khoản của người dùng khỏi hệ thống.
Điều kiện tiên quyết:

Người dùng đã đăng nhập vào hệ thống và có quyền truy cập vào chức năng "Đăng xuất và xóa tài khoản".

Kết quả:

Người dùng đã đăng xuất khỏi hệ thống hoặc tài khoản của họ đã bị xóa khỏi hệ thống.
# REQ-14: hệ thống có chức năng thanh toán nhiều hình thức

Mô tả chung:
Khách hàng có thể thanh toán cho đơn hàng của mình bằng nhiều hình thức khác nhau, bao gồm thanh toán trực tuyến qua các cổng thanh toán điện tử hoặc thanh toán khi nhận hàng.

Các bước thực hiện:

-	Khách hàng chọn sản phẩm mình muốn mua và thêm vào giỏ hàng.
-	Khách hàng đi đến trang thanh toán và chọn hình thức thanh toán mong muốn.
-	Nếu khách hàng chọn thanh toán trực tuyến, hệ thống sẽ chuyển họ đến trang của cổng thanh toán điện tử để thực hiện thanh toán.
-	Nếu khách hàng chọn thanh toán khi nhận hàng, họ sẽ được yêu cầu cung cấp thông tin về địa chỉ nhận hàng và thời gian giao hàng.
-	Sau khi hệ thống xác nhận thanh toán thành công, đơn hàng sẽ được xác nhận và giao hàng sẽ được tiến hành.
Điều kiện tiên quyết:

Khách hàng đã thêm sản phẩm vào giỏ hàng và đã chuyển đến trang thanh toán.
Hệ thống đã được cấu hình để hỗ trợ các hình thức thanh toán khác nhau.
Kết quả:

Khách hàng có thể thanh toán cho đơn hàng của mình bằng nhiều hình thức khác nhau, tùy thuộc vào sự lựa chọn của họ.
Đơn hàng sẽ được xác nhận và giao hàng sẽ được tiến hành sau khi thanh toán được xác nhận thành công.
# REQ-15: hệ thống có chức năng báo lỗi cho quản trị viên

Mô tả chung:
-	Chức năng này cho phép người dùng báo lỗi về các vấn đề liên quan đến hệ thống cho quản trị viên. Người dùng có thể báo cáo các lỗi liên quan đến sản phẩm, thanh toán, đăng nhập, đăng ký, tìm kiếm, sắp xếp, v.v. và cung cấp thông tin chi tiết về lỗi để quản trị viên có thể giải quyết vấn đề.

Các bước thực hiện:

-	Người dùng truy cập vào phần báo lỗi trên giao diện người dùng hoặc ở phần thông tin liên hệ trên trang web.
-	Người dùng cung cấp thông tin chi tiết về lỗi bao gồm loại lỗi, mô tả lỗi và bất kỳ thông tin liên quan nào, chẳng hạn như trang web hoặc sản phẩm bị ảnh hưởng, thời gian xảy ra lỗi, v.v.
-	Người dùng có thể cung cấp thông tin liên lạc để quản trị viên có thể liên hệ lại nếu cần.
-	Hệ thống ghi lại thông tin báo cáo lỗi và thông báo cho quản trị viên.
Điều kiện tiên quyết:
Người dùng phải có quyền truy cập vào chức năng báo lỗi để thực hiện chức năng này.

Kết quả:
Sau khi báo cáo lỗi thành công, quản trị viên có thể tiếp nhận và giải quyết vấn đề. Nếu cần, quản trị viên có thể liên hệ lại với người dùng để yêu cầu thêm thông tin hoặc cung cấp các giải pháp cho vấn đề báo cáo.


## ii. Use Case Diagram
