# BÀI TẬP THỰC HÀNH TỔNG HỢP

## 1. Báo cáo thiết kế giải pháp

**Mục tiêu:** Xây dựng chuỗi Prompt Chaining để tự động hóa việc hỗ trợ học tập bằng phương pháp Feynman và chấm bài theo Rubric.

**Dữ liệu đầu vào (Input):**
- Nội dung bài học.
- Câu trả lời của sinh viên.
- Tiêu chí và thang điểm Rubric.

**Kết quả đầu ra (Output):**
- Nội dung giải thích dễ hiểu theo phương pháp Feynman.
- Bảng chấm điểm theo từng tiêu chí.
- Tổng điểm và nhận xét.
- Gợi ý cải thiện kiến thức.

**Quy trình xử lý:**

1. Prompt 1: Kiểm tra và phân loại dữ liệu đầu vào.
2. Prompt 2: Giải thích kiến thức theo phương pháp Feynman.
3. Prompt 3: Đánh giá câu trả lời theo Rubric.
4. Prompt 4: Tổng hợp kết quả và kiểm tra lỗi trước khi xuất báo cáo.

## 2. Prompt hệ thống và các bước thực thi

### Prompt 1: Kiểm tra dữ liệu đầu vào

Bạn là trợ lý kiểm tra dữ liệu học tập.

Hãy kiểm tra 3 thông tin:
- Nội dung bài học.
- Câu trả lời của sinh viên.
- Rubric chấm điểm.

Nếu thiếu dữ liệu nào, hãy thông báo và yêu cầu bổ sung.
Nếu dữ liệu bị trống hoặc sai định dạng, không tiếp tục xử lý.
Nếu dữ liệu đầy đủ, chuyển sang bước giải thích kiến thức.

Không tự ý tạo thêm dữ liệu.

### Prompt 2: Giải thích theo phương pháp Feynman

Bạn là gia sư AI sử dụng phương pháp Feynman.

Dựa vào nội dung bài học đã được kiểm tra:
- Giải thích kiến thức bằng ngôn ngữ đơn giản.
- Chia nội dung thành các ý chính.
- Đưa ra ví dụ thực tế.
- Chỉ ra phần kiến thức quan trọng cần ghi nhớ.



### Prompt 3: Chấm bài theo Rubric

Bạn là trợ lý chấm bài tự động.

Hãy đọc câu trả lời của sinh viên và đối chiếu với Rubric.

Yêu cầu:
- Chấm điểm theo từng tiêu chí.
- Ghi rõ điểm tối đa và điểm đạt được.
- Nhận xét ưu điểm và lỗi sai.
- Không tự ý thay đổi thang điểm.
- Không chấm điểm nếu thiếu câu trả lời hoặc Rubric.
- Nếu câu trả lời không liên quan, cần thông báo rõ.

Kết quả trình bày dưới dạng bảng.

### Prompt 4: Tổng hợp kết quả

Bạn là trợ lý tổng hợp kết quả học tập.

Hãy tổng hợp kết quả từ các bước trước thành báo cáo gồm:

1. Nội dung giải thích theo Feynman.
2. Bảng chấm điểm theo Rubric.
3. Tổng điểm.
4. Nhận xét chung.
5. Hướng cải thiện.



## 3. Kết quả chạy thử

**Dữ liệu đầu vào:**

- Nội dung bài học: Khái niệm trí tuệ nhân tạo (AI).
- Câu trả lời: AI là công nghệ giúp máy tính thực hiện những công việc cần trí thông minh của con người như nhận diện hình ảnh và trả lời câu hỏi.
- Rubric:
  - Đúng kiến thức: 4 điểm.
  - Đầy đủ nội dung: 3 điểm.
  - Ví dụ minh họa: 2 điểm.
  - Trình bày rõ ràng: 1 điểm.

**Kết quả AI phản hồi:**

### 3.1. Giải thích theo phương pháp Feynman

AI là công nghệ giúp máy tính thực hiện những công việc thường cần đến trí thông minh của con người. Ví dụ, AI có thể nhận diện khuôn mặt, trả lời câu hỏi và phân tích dữ liệu.

### 3.2. Bảng chấm điểm

| Tiêu chí | Điểm tối đa | Điểm đạt |
|---|---:|---:|
| Đúng kiến thức | 4 | 4 |
| Đầy đủ nội dung | 3 | 2 |
| Ví dụ minh họa | 2 | 1 |
| Trình bày rõ ràng | 1 | 1 |
| **Tổng điểm** | **10** | **8** |

### 3.3. Nhận xét chung

Câu trả lời đúng kiến thức cơ bản, trình bày rõ ràng nhưng nội dung chưa đầy đủ. Phần ví dụ minh họa còn hạn chế.

### 3.4. Hướng cải thiện

Bổ sung thêm ví dụ thực tế về ứng dụng AI và giải thích cụ thể hơn để bài làm đầy đủ hơn.

## 4. Kết quả kiểm tra lỗi

- Dữ liệu đầu vào đầy đủ.
- Không phát hiện trường dữ liệu bị trống.
- Các tiêu chí chấm điểm được giữ nguyên.
- Tổng điểm 8/10, đúng với tổng điểm các tiêu chí.
- Kết quả đầu ra đầy đủ, không có lỗi định dạng.

