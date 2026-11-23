# BÀI TẬP: KHẮC PHỤC LỖI KHAI BÁO BIẾN SỐ TRONG PROMPT MẪU

## Bước 1: Phân tích lỗi

**Prompt lỗi:**

```text
Hãy viết một bài chia sẻ về Quản trị Prompt & System Instructions bằng ngôn ngữ [language]. Dành cho đối tượng {audience}.
```

**Các lỗi phát hiện:**

- Sử dụng hai kiểu ký hiệu biến khác nhau: `[language]` và `{audience}`.
- Tên biến chưa được viết hoa và chưa thống nhất cách đặt tên.
- AI hoặc hệ thống tự động hóa có thể khó nhận diện chính xác các vị trí cần thay thế dữ liệu.
- Gây khó khăn khi tái sử dụng Prompt Template và quản lý biến số.

## Bước 2: Đồng bộ biến số

**Prompt sau khi sửa:**

```text
Hãy viết một bài chia sẻ về Quản trị Prompt & System Instructions bằng ngôn ngữ [NGÔN_NGỮ]. Dành cho đối tượng [ĐỐI_TƯỢNG].
```

**Các biến số đã chuẩn hóa:**

| Biến số | Ý nghĩa |
|---|---|
| `[NGÔN_NGỮ]` | Ngôn ngữ sử dụng để viết bài |
| `[ĐỐI_TƯỢNG]` | Đối tượng tiếp nhận nội dung |

## Bước 3: Điền dữ liệu thực tế vào biến số

**Dữ liệu đầu vào:**

- `[NGÔN_NGỮ]` = Tiếng Việt
- `[ĐỐI_TƯỢNG]` = Sinh viên năm nhất ngành Công nghệ thông tin

**Prompt sau khi điền biến:**

```text

"Hãy viết một bài chia sẻ về Quản trị Prompt & System Instructions bằng ngôn ngữ [NGÔN_NGỮ]. Dành cho đối tượng [ĐỐI_TƯỢNG]."

Hãy thay thế các biến bằng dữ liệu thực tế:
- [NGÔN_NGỮ] = Tiếng Việt
- [ĐỐI_TƯỢNG] = Sinh viên năm nhất ngành Công nghệ thông tin

Yêu cầu:
1. Hiển thị Prompt sau khi đã thay thế biến.
2. Thực hiện Prompt và tạo bài chia sẻ.
3. Nội dung ngắn gọn, dễ hiểu, phù hợp với sinh viên năm nhất.
4. Không viết lời chào xã giao.
```

## Bước 4: Kết quả chạy thử

```
1. Quản trị Prompt là gì?
Quản trị Prompt là quá trình xây dựng, tổ chức, lưu trữ và cải thiện các câu lệnh (Prompt) để AI hiểu đúng yêu cầu và đưa ra kết quả chính xác.

Một Prompt tốt cần có yêu cầu rõ ràng, đầy đủ thông tin và xác định được kết quả mong muốn.
2. System Instructions là gì?
System Instructions là những chỉ dẫn nền tảng quy định vai trò, nhiệm vụ, cách phản hồi và giới hạn hoạt động của AI.

Ví dụ: Thiết lập AI đóng vai trò là trợ lý lập trình, giải thích kiến thức Python bằng ngôn ngữ đơn giản và phù hợp với người mới học.
3. Vai trò và lợi ích
Việc quản trị Prompt và System Instructions mang lại nhiều lợi ích:
- Tiết kiệm thời gian: Giúp AI hiểu yêu cầu nhanh hơn.
- Tăng độ chính xác: Hạn chế câu trả lời sai hoặc không đúng trọng tâm.
- Tạo tính nhất quán: Giúp AI duy trì phong cách và cách phản hồi theo yêu cầu.
- Tái sử dụng: Có thể lưu các Prompt hữu ích để sử dụng nhiều lần.
- Tăng hiệu quả học tập: Hỗ trợ sinh viên tìm hiểu kiến thức và giải quyết bài tập.
4. Ví dụ thực tế
Thay vì viết Prompt chung chung:
Giải thích Python.


Có thể viết Prompt rõ ràng hơn:
Bạn là trợ lý học tập ngành Công nghệ thông tin.

Hãy giải thích khái niệm biến trong Python
cho sinh viên năm nhất chưa có kiến thức lập trình.

Yêu cầu:
- Sử dụng ngôn ngữ đơn giản.
- Có ví dụ minh họa.
- Giải thích từng dòng code.
- Không sử dụng kiến thức nâng cao.


Kết quả nhận được sẽ cụ thể và phù hợp với nhu cầu học tập hơn.
5. Kết luận
Quản trị Prompt và System Instructions là kỹ năng quan trọng khi làm việc với AI. Đối với sinh viên năm nhất ngành Công nghệ thông tin, việc biết cách viết Prompt rõ ràng, thiết lập chỉ dẫn phù hợp và kiểm tra kết quả sẽ giúp học tập hiệu quả hơn, đồng thời xây dựng nền tảng tốt để ứng dụng AI trong công việc sau này.
```
