================================================================================
Công cụ EDA thường dùng trong thiết kế và kiểm thử
================================================================================

Để thiết kế và kiểm thử vi mạch, kỹ sư cần sử dụng các công cụ EDA (Electronic Design Automation).  
Với mức junior, việc nắm cơ bản cách dùng và mục đích của các công cụ này là rất quan trọng.  

Mô phỏng RTL (Simulation)
----------------------------
- **Mentor QuestaSim/ModelSim**: mô phỏng Verilog/VHDL, phổ biến trong kiểm thử.  
- **Synopsys VCS**: hiệu năng cao, dùng trong công ty lớn.  
- **Xilinx Vivado Simulator**: miễn phí khi làm FPGA.  

Thiết kế tổng hợp (Synthesis)
--------------------------------
- **Synopsys Design Compiler**: chuẩn công nghiệp để tổng hợp RTL thành gate-level netlist.  
- **Cadence Genus**: công cụ tổng hợp hiệu năng cao.  
- **Xilinx Vivado / Intel Quartus**: tổng hợp cho FPGA.  

Place and Route (P&R)
------------------------
- **Cadence Innovus**: dùng cho ASIC, thực hiện layout chi tiết.  
- **Synopsys IC Compiler II (ICC2)**: công cụ P&R mạnh mẽ.  
- **FPGA tools**: Vivado, Quartus hỗ trợ cả P&R trên FPGA.  

Kiểm thử nâng cao (Verification)
-----------------------------------
- **UVM (Universal Verification Methodology)** chạy trên simulator.  
- **Formal Verification (JasperGold, VC Formal)**: kiểm tra tính đúng đắn bằng chứng minh toán học.  
- **Linting tools (SpyGlass, AscentLint)**: phát hiện lỗi coding style, lỗi reset, latch.  

Quản lý waveform
-------------------
- **GTKWave**: miễn phí, dễ dùng cho waveform cơ bản.  
- **SimVision (Cadence)**: hỗ trợ debug mạnh.  
- **DVE (Synopsys)**: tích hợp với VCS.  

Quản lý dự án và code
------------------------
- **Git**: quản lý version, hợp tác nhóm.  
- **Makefile/Python scripts**: tự động hóa mô phỏng và regression.  
- **Jenkins**: chạy kiểm thử liên tục (CI/CD).  

Kết luận chương
-----------------
Junior nên bắt đầu bằng cách làm quen với simulator (QuestaSim, Vivado) và công cụ quản lý code (Git).  
Việc nắm các công cụ cơ bản này sẽ giúp dễ dàng hòa nhập vào dự án thực tế, trước khi học các công cụ nâng cao cho ASIC.
