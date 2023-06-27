Tên dataset: Dữ liệu việc làm vietnamworks.com
Nguồn thu thập: https://www.vietnamworks.com/
Ngày thu thập: 06/5/2023
Người thu thập:Lê Tuấn Cường-20520145@gm.uit.edu.vn
Mô tả:
	Bộ dữ liệu về việc làm từ nhiều ngành nghề được đăng lên trang web vietnamworks.Được thu thập nhằm mục đích đánh giá tổng quan về sự phân bố công việc, mức lương các lĩnh vực nghề
Bộ dữ liệu gồm 9555 dòng với 14 thuộc tính:
	1) comp_name: tên công ty đăng tải (string)
	2) tittle_job:	tiêu đề công việc (string)
	3) local: vị trí công ty (list[string])
	4) date: ngày đăng tải	(datetime)
	5) level: cấp bậc cần tuyển dụng (string)	gồm 5 cấp bậc:
		+ Mới Tốt Nghiệp
		+ Giám Đốc và Cấp Cao Hơn
		+ Nhân viên
		+ Trưởng phòng
		+ Thực tập sinh/Sinh viên
	6) industry: lĩnh vực công việc (list[num])
		
		2:	An toàn lao động
		3:	Biên phiên dịch
		4:	Bác sĩ
		5:	Bán buôn - Bán lẻ - Quản lý cửa hàng
		6:	Bảo hiểm
		7:	Bất động sản
		8:	Chăm sóc khách hàng
		9:	Cơ khí
		10:	Cấp quản lý điều hành
		
		12:	Dược Phẩm - Công nghệ sinh học
		13:	Dược sĩ
		14:	Dệt may - Da giày
		15:	Giáo dục - Đào tạo
		16:	Hàng hải
		17:	Hàng không  - Du lịch
		18:	Hành chính - Thư ký
		19:	Hóa học - Hóa sinh
		20:	IT Phần cứng - Mạng - Viễn Thông
		21:	IT Phần mềm
		22:	Internet - Online Media
		23:	Khai thác năng lượng - Khoáng sản
		
		25:	Khách sạn - Nhà hàng - Du lịch
		
		27:	Kiến trúc - Thiết kế nội thất
		28:	Kiểm toán
		29:	Kế toán
		30:	Marketing
		31:	Môi trường - Xử lý chất thải
		32:	Nghề nghiệp khác
		33:	Ngân hàng
		34:	Nhân sự
		35:	Nông - Lâm - Ngư nghiệp
		36:	Phi chính phủ - Phi lợi nhuận
		37:	Pháp Lý - Tuân thủ
		38:	Quản lý dự án
		39:	Quản lý tiêu chuẩn và chất lượng
		40:	Quảng cáo - Khuyến mãi - Đối ngoại
		41:	Sản phẩm công nghiệp
		42:	Sản xuất - Lắp ráp - Chế biến
		43:	Thiết kế - Sáng tạo nghệ thuật
		44:	Thu mua - Kho Vận - Chuỗi cung ứng
		45:	Thông tin - Truyền thông - Xuất bản - In ấn
		46:	Thương mại điện tử
		47:	Thời trang
		48:	Thực phẩm - Đồ uống
		49:	Trình dược viên
		50:	Tài chính - Đầu tư
		51:	Tài chính công nghệ
		52:	Tư vấn
		53:	Tự động hóa - Ô tô
		54:	Vận Tải - Lái xe - Giao nhận
		55:	Vận hành máy - Bảo trì - Bảo dưỡng thiết bị
		56:	Xuất Nhập Khẩu
		57:	Xây dựng
		58:	Y tế - Chăm sóc sức khỏe
		59:	Điện lạnh - Nhiệt lạnh
		60:	Điện - Điện tử
		61:	Bán hàng kỹ thuật
		62:	Công nghệ cao
		63:	Hàng cao cấp
		64:	Hàng gia dụng
		65:	Hàng tiêu dùng
		66:	Mới tốt nghiệp
		67:	Người nước ngoài - Việt Kiều
		68:	Overseas Jobs
		69:	Thời vụ - Hợp đồng ngắn hạn
	7) skills: kĩ năng yêu cầu (string)	
	8) description: mô tả công việc (string)	
	9) requirement: yêu cầu công việc (string)
	10) welfare: phúc lợi công việc(string)
	11) min_salary: tiền lương tối thiểu (int)	
	12) max_salary: tiền lương tối đa (int)	
	13) min_year: số năm kinh nghiệm tối thiểu (float)	
	14) max_year: số năm kinh nghiệm tối đa (float)
Chú ý:
	2 cột min_year và max_year được phát hiện bằng công cụ thông qua cột requirement nên tính đảm bảo không được chính xác.
	giá trị min_salary và max_salary ban đầu là đơn vị $. Sau khi tiền xử lý đã chuyển sang VND theo tỉ lệ 1:24600 
