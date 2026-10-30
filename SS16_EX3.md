
**Vấn đề :**
-Các thông báo kỹ thuật về cảm biến bị lẫn lộn giữa các tin nhắn tán gẫu và meme hài hước
-Thành viên thường xuyên quên deadline vì tin nhắn bị đè nát.
**Yêu cầu:**
Thiết kế cấu trúc Channels / Topics cho dự án trên Lark hoặc Slack để tách biệt thảo luận kỹ thuật, thông báo và giải trí.

## 1. Sơ đồ kiến trúc kênh (Channel Architecture trên Lark / Slack)

Cấu trúc các kênh được phân chia rõ ràng theo tiền tố (prefix) để tự động định hướng thông tin, tránh việc tin nhắn kỹ thuật bị đè lấp bởi meme hay tán gẫu:
|Quyền đăng tin|nội dung thông tin|
|:---|:---|
|Admin |Lịch họp sprint, deadline toàn dự án, thông báo thay đổi quan trọng|
|Tất cả thành viên|Thảo luận phần cứng: Cảm biến siêu âm/hồng ngoại,đấu nối thiết bị tại bãi xe thực tế.|
|Tất cả thành viên|Thảo luận phần mềm: Xử lý luồng nhận diện biển s|
|Tất cả thành viên|Khu vực giải trí: Chia sẻ meme, chém gió, rủ rê ăn uống, giải tỏa căng thẳng ngoài lề dự án.|

Bản quy ước giao tiếp: 3 quy tắc vàng để tránh No-Hello Trap và spam @all.
-Quy tắc 1:Cấm "No-Hello":
 Gửi ngay toàn bộ ngữ cảnh trong **1 tin nhắn duy nhất** để người đọc có thể xử lý ngay khi rảnh
-Quy tắc 2: Kiểm soát chặt chẽ thẻ tag: 
No sử dụng `@all`,  `@channel`,  trong các channel kỹ thuật và giải trí.
-Quy tắc 3: Bắt buộc sử dụng "Reply in Thread:
Một vấn đề cụ thể **phải được gom vào khung** của tin nhắn gốc.
Khung chat chính  chỉ dùng để phát đi chủ đề mới, giúp giao diện luôn sạch sẽ và không bị trôi các thông báo quan trọng.


