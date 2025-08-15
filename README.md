# Sách Thiết Kế và Kiểm Tra Thiết Kế
Yêu cầu: Có kiến thức nền cơ bản về kỹ thuật số và mạch điện (chuyên ngành điện tử hoặc tương đương)
Cấp độ: người mới học lĩnh vực thiết kế số

# Cài đặt Sphinx
Trang chủ của [Sphinx](https://www.sphinx-doc.org)
```
pip install sphinx
```

# Cài đặt các phần mở rộng
Định dạng sách
```
pip install sphinx_rtd_theme
```

Chuyển ảnh từ svg sang pdf
```
pip install sphinxcontrib-svg2pdfconverter
```

Chèn waveform được tạo ra bởi Wavedrom
```
pip install sphinxcontrib-wavedrom
```

# Biên dịch sách (build)
Sử dụng câu lệnh bên dưới trong thư mục chứa sách
```
make html
```

