========================================
Quy trình thiết kế vi mạch số
========================================

Trong chương này, chúng ta sẽ tìm hiểu quy trình thiết kế vi mạch số (Digital IC Design Flow) – từ ý tưởng ban đầu cho đến sản phẩm cuối cùng. Đây là kiến thức nền tảng mà bất kỳ kỹ sư mới (junior) nào cũng cần nắm rõ.

Ý tưởng và đặc tả (Specification)
------------------------------------
- Xuất phát từ yêu cầu hệ thống: cần chip làm gì, tốc độ bao nhiêu, tiêu thụ điện năng ra sao.
- Đặc tả (spec) là tài liệu mô tả chi tiết chức năng, giao tiếp, chuẩn cần tuân thủ.
- Đây là đầu vào quan trọng nhất, quyết định toàn bộ thiết kế sau này.

Viết RTL (Register Transfer Level)
-------------------------------------
- Dùng HDL như **Verilog** hoặc **VHDL** để mô tả mạch ở mức thanh ghi.
- RTL mô tả dữ liệu di chuyển và xử lý trong mạch theo từng chu kỳ xung nhịp.
- Đây là bước chính của kỹ sư thiết kế (Design Engineer).

Xác minh chức năng (Functional Verification)
------------------------------------------------
- Viết testbench để kiểm tra RTL có hoạt động đúng với đặc tả không.
- Sử dụng mô phỏng để phát hiện lỗi logic.
- Đây là công việc chính của kỹ sư kiểm thử (Verification Engineer).

Tổng hợp (Synthesis)
-----------------------
- Biến mã RTL thành cổng logic (gate-level netlist).
- Công cụ EDA (Electronic Design Automation) sẽ ánh xạ RTL sang thư viện cell chuẩn.
- Kiểm tra các ràng buộc về thời gian (timing constraints).

Thiết kế vật lý (Physical Design)
------------------------------------
- Chuyển netlist thành layout (bố trí transistor, dây nối trên silicon).
- Các bước: Floorplanning, Placement, Routing, Timing Closure.
- Đầu ra là file GDSII dùng cho chế tạo chip.

Chế tạo và kiểm thử (Fabrication & Testing)
-----------------------------------------------
- Gửi layout tới nhà máy (foundry) để sản xuất.
- Kiểm thử chip thật (post-silicon validation).
- Nếu đạt yêu cầu thì đưa vào sản xuất hàng loạt.

Kết luận chương
-----------------
Quy trình thiết kế vi mạch số gồm nhiều bước, từ đặc tả đến chế tạo. Người mới cần hiểu rõ từng bước để biết mình sẽ tham gia ở giai đoạn nào (design, verification hay physical design). Những chương tiếp theo sẽ đi sâu vào chi tiết RTL, testbench và phương pháp kiểm thử.
