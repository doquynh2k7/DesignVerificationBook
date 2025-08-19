================================================================================
Giới thiệu tổng quan
================================================================================

Trong chương đầu tiên này, chúng ta sẽ làm quen với những khái niệm cơ bản nhất về vi mạch, lĩnh vực thiết kế (design) và kiểm thử (verification). Đây là nền tảng quan trọng để người mới bắt đầu có một cái nhìn tổng thể trước khi đi sâu hơn vào các bước kỹ thuật.

Vi mạch là gì?
-----------------
- Vi mạch (Integrated Circuit – IC) là tập hợp hàng triệu đến hàng tỷ transistor được tích hợp trên một chip bán dẫn.
- IC có nhiều loại: vi xử lý (CPU), bộ nhớ (RAM, ROM, Flash), chip giao tiếp (I/O), chip điều khiển, v.v.
- Vai trò quan trọng trong hầu hết các thiết bị điện tử: từ điện thoại, máy tính, xe hơi đến thiết bị IoT.

Thiết kế vi mạch (Design)
-----------------------------
- Là quá trình tạo ra phần cứng theo yêu cầu, bắt đầu từ đặc tả (specification).
- Sử dụng các ngôn ngữ mô tả phần cứng (HDL – Hardware Description Language) như **Verilog** hoặc **VHDL**.
- Bao gồm nhiều bước: viết RTL, tổng hợp (synthesis), layout, chế tạo.

Kiểm thử và xác minh (Verification)
---------------------------------------
- Đảm bảo mạch thiết kế đúng với đặc tả và không có lỗi.
- Chiếm khoảng 60-70% thời gian trong một dự án vi mạch.
- Phương pháp phổ biến: viết testbench, mô phỏng (simulation), dùng các ngôn ngữ hỗ trợ như SystemVerilog/UVM.

Tại sao người mới cần học cả design và verification?
--------------------------------------------------------
- Người làm junior cần nắm khái niệm cơ bản cả hai mảng để hiểu quy trình.
- Tùy định hướng nghề nghiệp có thể đi sâu vào thiết kế hoặc kiểm thử.
- Khi hiểu cả hai, dễ phối hợp trong nhóm và giảm sai sót.

Kết luận chương
-----------------
Chương này cung cấp bức tranh toàn cảnh về vi mạch, thiết kế và kiểm thử. Các chương tiếp theo sẽ đi sâu vào chi tiết từng giai đoạn, giúp người mới xây dựng kỹ năng thực tế.
