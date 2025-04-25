
# bài tập 6 của sv:mssv k225480106002 - nguyễn tuấn anh - hệ quản trị csdl
## Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

DEADLINE: 23H59:59 NGÀY 25/4/2025

## Bài làm 

1: Các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
- Bước 1: mở SQL Server Management Studio 20
- Bước 2: click connect
- bước 3: tạo database mới ==> database mới của em tên là SV_TNUT
  ![Screenshot (271)](https://github.com/user-attachments/assets/f6898767-58c6-4c8c-9b04-968aee4c8f52)

- Bước 4: Tạo Query mới:
![Screenshot (272)](https://github.com/user-attachments/assets/5090ec33-b24d-497f-a333-63f026c6aa91)

- Bước 5: em lấy dữ liệu từ file sv_tnut.sql của thầy và ấn Execute
  ![Screenshot (274)](https://github.com/user-attachments/assets/98aeaedd-fb4b-4e77-810a-d79d3b26b686)

2. dữ liệu đầu vào của em (em là sinh viên đang làm bài tập của thầy cốp 100% không clone của ai)
Câu lệnh SQL sẽ:

Lấy toàn bộ thông tin của sinh viên từ bảng SV

Nhưng chỉ những người có:

Tên là "Anh"

Ngày sinh là 18/12/2004

Số điện thoại là 919668434
   ![Screenshot (277)](https://github.com/user-attachments/assets/2d50ee71-096d-4100-b9e9-6c9802b66321)

3. nhập sql để tìm xem có những sv nào trùng ngày/tháng/năm với em:
   → Lấy toàn bộ thông tin của sinh viên từ bảng SV,
nhưng chỉ những người có ngày, tháng, năm sinh là 18/12/2004.

   ![Screenshot (278)](https://github.com/user-attachments/assets/c889d42a-b515-42cf-8ad7-f01e3f60201b)

4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em:
Câu lệnh SQL trên sẽ:

→ Lấy toàn bộ thông tin của sinh viên từ bảng SV
→ Nhưng chỉ những người sinh vào ngày 18 tháng 12 (năm nào cũng được).
    ![Screenshot (279)](https://github.com/user-attachments/assets/0c13f8c1-c434-4193-9b19-37738b8b3db0)

5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em:
   Câu lệnh SQL trên sẽ:

→ Lấy toàn bộ thông tin của sinh viên từ bảng SV
→ Nhưng chỉ những người sinh vào tháng 12 năm 2004.

   ![Screenshot (280)](https://github.com/user-attachments/assets/68d5345b-855c-4dc8-91d7-03fba4103681)

6. nhập sql để tìm xem có những sv nào trùng tên với em:

    Câu lệnh SQL trên sẽ:

→ Lấy toàn bộ thông tin của sinh viên từ bảng SV
→ Nhưng chỉ những người có tên là "Anh".

![Screenshot (281)](https://github.com/user-attachments/assets/bc3ba68d-6143-41b2-b623-9588df86af72)

7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.

Câu lệnh SQL trên sẽ:

→ Lấy toàn bộ thông tin sinh viên từ bảng SV
→ Nhưng chỉ những người có họ đệm là "Nguyễn Tuấn"

![Screenshot (282)](https://github.com/user-attachments/assets/31922eb5-b4f1-4aad-8378-5d5cc7a541bd)

8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
   Câu SQL trên sẽ:

→ Lấy số điện thoại sdt của sinh viên từ bảng SV
→ So sánh từng ký tự trong số điện thoại với chuỗi chuẩn: '916684344'
→ Nếu ký tự nào không đúng, thì cộng thêm 1 lỗi
→ Tổng lỗi được đặt tên là so_ky_tu_sai
→ Cuối cùng sắp xếp kết quả theo số ký tự sai tăng dần

![Screenshot (284)](https://github.com/user-attachments/assets/88853581-68f7-4527-935b-23a67c20a98e)

9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH:
    Câu SQL trên sẽ:

→ Lấy thông tin các sinh viên từ bảng Esv_tnut, bao gồm mã sinh viên, họ, tên, trường, lớp học, và số điện thoại.
→ Lọc những sinh viên thuộc lớp có tên chứa chuỗi "KMT".
→ Lấy tối đa 10.000 bản ghi thỏa mãn điều kiện trên.
→ Sắp xếp kết quả theo tên ([ten]) và họ ([hodem]) theo chuẩn tiếng Việt, phân biệt chữ hoa, chữ thường và dấu tiếng Việt.

![Screenshot (286)](https://github.com/user-attachments/assets/415427c5-6cee-4c7a-937e-8d86bad00ba1)

10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VƯỚNG MẮC)
- Thưa thầy rằng là!! câu 10 này em làm theo kiêu như này ạ: em ngồi em đọc file của thầy, em đọc thấy tên ai là nữ thì em lấy ạ , do em chưa hiểu biết nhiều nên chỉ có thể làm như thế thôi ạ.

![Screenshot (287)](https://github.com/user-attachments/assets/a742a980-3a9f-41a9-bfc5-855b9f9bf834)
