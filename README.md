# my_flutter_app

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


lib/
├── main.dart
├── core/
│   ├── constants/       # Hằng số dùng toàn app (màu sắc, API keys...)
│   ├── utils/           # Hàm tiện ích chung
│   ├── services/        # Dịch vụ kết nối Supabase, Storage, Noti...
│   └── theme/           # Giao diện, font, màu sắc dùng chung
├── data/
│   ├── models/          # Định nghĩa các class như Message, User, ChatRoom...
│   ├── repositories/    # Tầng gọi API / database (giao tiếp Supabase)
├── features/
│   ├── auth/            # Đăng nhập, đăng ký, xác thực
│   │   ├── screens/
│   │   ├── widgets/
│   │   └── controller/  # State & logic xử lý auth
│   ├── chat/
│   │   ├── screens/     # ChatPage, ChatDetail, NewMessagePage,...
│   │   ├── widgets/     # MessageBubble, ChatInput, ChatHeader...
│   │   ├── controller/  # State / logic chat
│   │   └── bindings/    # Khởi tạo controller (nếu dùng GetX)
│   └── contacts/        # Tính năng danh bạ, tìm người dùng, tạo nhóm
├── routes/
│   └── app_routes.dart  # Định nghĩa đường dẫn các màn hình
└── shared/
    ├── widgets/         # Các widget dùng chung (Button, Avatar, Loading...)
    ├── extensions/      # Hàm mở rộng cho String, DateTime...
    └── mixins/          # Logic tái sử dụng
