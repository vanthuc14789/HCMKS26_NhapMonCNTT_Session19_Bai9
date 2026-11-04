---


---

<h1 id="bài-tập-quản-lý-mật-khẩu-pixelforge-studio">BÀI TẬP: QUẢN LÝ MẬT KHẨU PIXELFORGE STUDIO</h1>
<h2 id="phần-1-phân-tích-an-ninh">PHẦN 1: PHÂN TÍCH AN NINH</h2>
<p>Câu 1. Vì sao lưu mật khẩu trên Chrome nguy hiểm?</p>
<ul>
<li>
<p>Mã độc Infostealer có thể tìm và đánh cắp dữ liệu trong tệp <code>Login Data</code>.</p>
</li>
<li>
<p>Có thể lấy mật khẩu, Cookie và thông tin đăng nhập.</p>
</li>
<li>
<p>Hacker có thể dùng mật khẩu bị lộ để tấn công các tài khoản khác.</p>
</li>
</ul>
<p>Kết luận: Không nên chỉ sử dụng Chrome để lưu mật khẩu quan trọng.</p>
<p>Câu 2. Zero-Knowledge và Client-side Decryption là gì?</p>
<ul>
<li>
<p>Zero-Knowledge: Nhà cung cấp không thể đọc mật khẩu của người dùng.</p>
</li>
<li>
<p>Client-side Decryption: Dữ liệu được giải mã ngay trên thiết bị người dùng.</p>
</li>
<li>
<p>AES-256: Thuật toán mã hóa dữ liệu bằng khóa 256 bit.</p>
</li>
</ul>
<p>Nếu máy chủ Bitwarden bị hack, hacker chỉ lấy được dữ liệu đã mã hóa nếu không có khóa giải mã.</p>
<h2 id="phần-2-thiết-kế-chính-sách">PHẦN 2: THIẾT KẾ CHÍNH SÁCH</h2>
<p>Câu 3. Tạo Master Passphrase</p>
<ul>
<li>
<p>Sử dụng ít nhất 6 từ ngẫu nhiên.</p>
</li>
<li>
<p>Dài tối thiểu 20 ký tự.</p>
</li>
<li>
<p>Không dùng tên hoặc ngày sinh.</p>
</li>
<li>
<p>Bật xác thực hai yếu tố (2FA).</p>
</li>
</ul>
<p>Ví dụ: <code>Free-FiRe-SOng-DaiHT</code></p>
<p>Đây chỉ là ví dụ, không nên dùng làm mật khẩu thật.</p>
<p>Câu 4. Cấu hình Bitwarden Generator</p>

<table>
<thead>
<tr>
<th>Thuộc tính</th>
<th>Cấu hình</th>
</tr>
</thead>
<tbody>
<tr>
<td>Độ dài</td>
<td>24 ký tự</td>
</tr>
<tr>
<td>Chữ hoa (A-Z)</td>
<td>Bật</td>
</tr>
<tr>
<td>Chữ thường (a-z)</td>
<td>Bật</td>
</tr>
<tr>
<td>Chữ số (0-9)</td>
<td>Bật</td>
</tr>
<tr>
<td>Ký tự đặc biệt</td>
<td>Bật</td>
</tr>
<tr>
<td>Số tối thiểu</td>
<td>1</td>
</tr>
<tr>
<td>Ký tự đặc biệt tối thiểu</td>
<td>1</td>
</tr>
</tbody>
</table><p>Mỗi tài khoản sử dụng một mật khẩu ngẫu nhiên riêng biệt.<br>
Câu 5. Vì sao Auto-fill chống Phishing?</p>
<ul>
<li>
<p>Bitwarden kiểm tra tên miền trước khi điền mật khẩu.</p>
</li>
<li>
<p>Không tự động điền trên website giả như <code>githúb.com</code>.</p>
</li>
<li>
<p>Giảm nguy cơ nhập mật khẩu vào trang web giả mạo.</p>
</li>
</ul>
<p>Câu 6. Quy trình lưu trữ Emergency Kit</p>
<ol>
<li>
<p>Thiết lập Trưởng nhóm làm liên hệ khẩn cấp.</p>
</li>
<li>
<p>Lưu mã khôi phục ở nơi an toàn.</p>
</li>
<li>
<p>In thông tin cần thiết và cất trong két sắt.</p>
</li>
<li>
<p>Thiết lập ít nhất hai quản trị viên cho Organization.</p>
</li>
<li>
<p>Kiểm tra quyền truy cập định kỳ 3 tháng/lần.</p>
</li>
</ol>
<h2 id="phần-3-kế-hoạch-triển-khai">PHẦN 3: KẾ HOẠCH TRIỂN KHAI</h2>
<ol>
<li>
<p>Tạo Bitwarden Organization cho studio.</p>
</li>
<li>
<p>Thêm 8 thành viên vào hệ thống.</p>
</li>
<li>
<p>Chuyển hơn 40 tài khoản vào két sắt.</p>
</li>
<li>
<p>Đổi mật khẩu thành chuỗi ngẫu nhiên tối thiểu 16 ký tự.</p>
</li>
<li>
<p>Bật 2FA và phân quyền truy cập.</p>
</li>
<li>
<p>Kiểm tra bảo mật định kỳ.</p>
</li>
</ol>

