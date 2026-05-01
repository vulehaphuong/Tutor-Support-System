# Tutor Support System
Project được làm dựa trên yêu cầu của bài tập lớn môn CNPM khóa 251, tập trung vào quy trình xây dựng 1 trang web/ứng dụng 
## 1. 📋Project Context
<p style="text-align: justify;">
Trong bối cảnh giáo dục đại học tại Việt Nam, đặc biệt tại Trường Đại học Bách Khoa – ĐHQG TP.HCM, nhu cầu hỗ trợ sinh viên trong quá trình học tập và phát triển kỹ năng ngày càng trở nên quan trọng. Số lượng sinh viên lớn, chương trình đào tạo có độ khó cao, cùng với sự khác biệt về nền tảng học tập và kỹ năng đầu vào khiến nhiều sinh viên gặp khó khăn trong việc thích nghi, duy trì kết quả học tập ổn định, cũng như phát triển các kỹ năng mềm cần thiết cho nghề nghiệp sau này. Bên cạnh đó, sự đa dạng về lĩnh vực chuyên môn và phương pháp học tập cũng đòi hỏi sinh viên phải có định hướng phù hợp và sự đồng hành kịp thời từ những người có kinh nghiệm. Vì lý do đó nên nhà trường đã triển khai chương trình hỗ trợ Tutor/Mentor như một giải pháp nhằm giúp sinh viên:
<p>

- Được định hướng học tập và phát triển kỹ năng mềm.
- Nhận hỗ trợ trực tiếp từ giảng viên, nghiên cứu sinh, hoặc sinh viên khóa trên có thành tích học tập tốt.
- Có cơ hội kết nối, trao đổi, và nhận sự đồng hành xuyên suốt hành trình học tập.

<p style="text-align: justify;">
Tuy nhiên, việc quản lý thủ công bằng các công cụ truyền thống (Excel, email,thông báo rời rạc) bộc lộ nhiều hạn chế:
<p>

- **Khó khăn trong quản lý thông tin:** hồ sơ sinh viên và tutor không tập trung, dễ bị sai lệch hoặc trùng lặp.
- **Quy trình đăng ký thiếu minh bạch:** sinh viên khó chọn hoặc ghép cặp với tutor phù hợp.
- **Khó khăn trong tổ chức buổi gặp gỡ:** sắp xếp lịch, hủy/đổi lịch và gửi thông báo mất nhiều thời gian, không đồng bộ.
- **Thiếu công cụ đánh giá và theo dõi:** sinh viên chưa có kênh chính thống để phản hồi; tutor khó theo dõi tiến độ; khoa và phòng ban thiếu dữ liệu tổng quan để đưa ra quyết định.
- **Thiếu tính mở rộng và tích hợp:** chưa kết nối với hạ tầng CNTT hiện có
của trường (HCMUT_SSO, HCMUT_DATACORE, HCMUT_LIBRARY).

<p style="text-align: justify;">
Chính vì vậy, một hệ thống hỗ trợ Tutor/Mentor hiện đại, hiệu quả và có khả năng
tích hợp sâu với hạ tầng sẵn có của trường là cần thiết, nhằm đảm bảo tính chính xác,
minh bạch, tiết kiệm thời gian, và nâng cao trải nghiệm cho tất cả các bên liên quan.
<p>

## 2. 🎯Mục tiêu dự án

### 2.1. Mục tiêu tổng quát
<p style="text-align: justify;">
Xây dựng và triển khai một hệ thống phần mềm quản lý chương trình Tutor/Mentor hiện đại, đồng bộ với hạ tầng công nghệ thông tin của Trường Đại học Bách Khoa – ĐHQG TP.HCM, nhằm:
<p>

- **Nâng cao hiệu quả** quản lý và vận hành chương trình Tutor/Mentor.
- **Tạo môi trường học tập tương tác**, hỗ trợ phát triển học thuật và kỹ năng mềm cho sinh viên.
- **Tối ưu hóa** công tác phân bổ nguồn lực và khai thác dữ liệu cho nhà trường.

### 2.2. Mục tiêu cụ thể
Dự án hướng đến các mục tiêu cụ thể sau:
- Xây dựng kho dữ liệu tập trung, đồng bộ và minh bạch (tích hợp HCMUT_SSO, HCMUT_DATACORE).
- Tạo quy trình đăng ký và ghép cặp thuận tiện, có hỗ trợ từ AI.
- Hình thành cơ chế quản lý lịch hẹn và buổi tư vấn linh hoạt, đồng bộ.
- Cung cấp công cụ phản hồi, đánh giá để nâng cao chất lượng chương trình.
- Mở rộng khả năng tích hợp với các hệ thống khác của nhà trường và phát triển cộng đồng học tập trực tuyến.

---

## 3. 🔎Phạm vi dự án

- **Phạm vi chức năng:** Tập trung quản lý toàn diện chương trình Tutor/Mentor: lưu trữ thông tin, quy trình đăng ký, kết nối sinh viên - tutor, giám sát và đánh giá hiệu quả.
- **Phạm vi người dùng:**
    - **Sinh viên:** Người tham gia nhận hỗ trợ.
    - **Tutor:** Người cố vấn, hướng dẫn.
    - **Cán bộ điều phối:** Giám sát, quản lý hoạt động.
    - **Đơn vị quản lý (Khoa/Phòng):** Khai thác dữ liệu để ra quyết định.
- **Phạm vi công nghệ:** Triển khai trên hạ tầng CNTT của HCMUT, tận dụng: HCMUT_SSO (xác thực), HCMUT_DATACORE (dữ liệu), và HCMUT_LIBRARY (tài nguyên học tập). Hướng tới khả năng mở rộng tích hợp các dịch vụ mới.

---

## 4. 🌐Các bên liên quan

| Bên liên quan | Vai trò chính | Mong đợi chính |
| :--- | :--- | :--- |
| **Sinh viên**         | Đối tượng trung tâm, tham gia tư vấn, phản hồi.| Đăng ký dễ dàng, tìm tutor phù hợp, nhận nhắc lịch, tiếp cận học liệu. |
| **Tutor**             | Hướng dẫn, cố vấn, quản lý mentee.             | Công cụ quản lý lịch đơn giản, minh chứng hoạt động, chia sẻ học liệu. |
| **Khoa/Bộ môn**       | Giám sát chất lượng, khai thác dữ liệu.        | Báo cáo minh bạch, công cụ phân tích dữ liệu học tập. |
| **Phòng Đào tạo**     | Quản lý tổng thể, phân bổ nguồn lực.           | Báo cáo tổng quan, đồng bộ dữ liệu, tự động hóa quy trình. |
| **Phòng CTSV**        | Ghi nhận sự tham gia (điểm RL, học bổng).      | Công cụ theo dõi mức độ tham gia, trích xuất dữ liệu nhanh. |
| **Phòng CNTT**        | Đảm bảo vận hành, an toàn thông tin.           | Khả năng tích hợp dễ dàng, bảo mật dữ liệu, hạn chế sai sót thủ công. |
| **Nhóm phát triển**   | Phân tích, thiết kế, phát triển và bảo trì.    | Hệ thống ổn định, tích lũy kinh nghiệm nghề nghiệp. |