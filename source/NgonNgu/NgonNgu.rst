=============================================
Ngôn ngữ mô tả phần cứng (HDL)
=============================================

Ngôn ngữ mô tả phần cứng (Hardware Description Language – HDL) là công cụ chính để thiết kế vi mạch số. Chương này giúp người mới làm quen với **Verilog** và **VHDL**, hai ngôn ngữ phổ biến nhất trong ngành.

Khái niệm cơ bản
-------------------
- HDL khác với ngôn ngữ lập trình (C, Python) ở chỗ:  
  + Mô tả phần cứng hoạt động song song.  
  + Mỗi dòng lệnh trong HDL có thể biểu diễn một mạch số thật.  
- Dùng để mô tả: logic, trạng thái, đường truyền dữ liệu.

Verilog
-----------
- Cú pháp gần với C, dễ học cho người mới.
- Cấu trúc cơ bản: `module`, `input`, `output`, `wire`, `reg`.
- Ví dụ:

.. code-block:: verilog

   module AND_gate (
       input a, b,
       output y
   );
       assign y = a & b;
   endmodule

- Dùng nhiều trong công nghiệp nhờ sự đơn giản và phổ biến.

VHDL
--------
- Ngôn ngữ có cú pháp chặt chẽ hơn, gần giống Ada.
- Cấu trúc: `entity` và `architecture`.
- Ví dụ:

.. code-block:: vhdl

   entity AND_gate is
       Port ( a : in STD_LOGIC;
              b : in STD_LOGIC;
              y : out STD_LOGIC);
   end AND_gate;

   architecture Behavioral of AND_gate is
   begin
       y <= a AND b;
   end Behavioral;

- Phù hợp với các dự án yêu cầu chuẩn hóa, đặc biệt ở châu Âu.

So sánh Verilog và VHDL
--------------------------
- Verilog: ngắn gọn, dễ học, phổ biến ở Mỹ và châu Á.  
- VHDL: chặt chẽ, mô tả chi tiết, phổ biến ở châu Âu.  
- Nhiều công ty hỗ trợ cả hai, nhưng xu hướng hiện nay thiên về Verilog/SystemVerilog.

Khái niệm RTL (Register Transfer Level)
------------------------------------------
- RTL mô tả cách dữ liệu di chuyển giữa các thanh ghi và cách xử lý logic.
- RTL là mức trừu tượng chính để viết code thiết kế.
- Cả Verilog và VHDL đều được dùng để viết RTL.

Kết luận chương 3
-----------------
HDL là nền tảng bắt buộc với kỹ sư vi mạch. Junior cần nắm chắc cú pháp cơ bản, hiểu sự khác biệt giữa Verilog và VHDL, và biết cách viết mô tả RTL đơn giản.
