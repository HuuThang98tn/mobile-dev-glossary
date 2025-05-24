# 🐦 Tổng Hợp Thuật Ngữ Trong Phát Triển Flutter

Tài liệu này tổng hợp các thuật ngữ phổ biến và quan trọng trong quá trình phát triển ứng dụng Flutter, chia theo từng nhóm chức năng để dễ học và sử dụng.

---

## 📦 1. Cốt lõi của Flutter

| Thuật ngữ                      | Mô tả                                                  |
| ------------------------------ | ------------------------------------------------------ |
| **Flutter**                    | SDK của Google để phát triển app đa nền tảng bằng Dart |
| **Dart**                       | Ngôn ngữ lập trình chính thức dùng cho Flutter         |
| **Widget**                     | Thành phần cơ bản để xây dựng giao diện trong Flutter  |
| **StatelessWidget**            | Widget không thay đổi theo thời gian                   |
| **StatefulWidget**             | Widget có thể thay đổi trạng thái                      |
| **Hot Reload**                 | Tính năng cập nhật UI ngay khi sửa code                |
| **BuildContext**               | Ngữ cảnh của widget trong cây widget                   |
| **MaterialApp / CupertinoApp** | App Flutter theo phong cách Android/iOS                |

---

## 🧩 2. Giao Diện & Layout

| Thuật ngữ                          | Mô tả                                          |
| ---------------------------------- | ---------------------------------------------- |
| **Column / Row / Stack**           | Bố cục cơ bản trong Flutter                    |
| **Container**                      | Widget đa năng chứa nội dung và định dạng      |
| **Padding / Margin / Align**       | Định vị và khoảng cách                         |
| **Scaffold**                       | Khung xương của màn hình: AppBar, body, FAB... |
| **ListView / GridView / PageView** | Hiển thị danh sách và trang                    |
| **ThemeData**                      | Quản lý chủ đề màu sắc, font... toàn app       |

---

## 🔁 3. Navigation & Routing

| Thuật ngữ                  | Mô tả                            |
| -------------------------- | -------------------------------- |
| **Navigator**              | Quản lý stack màn hình           |
| **Named Routes**           | Định nghĩa route theo tên        |
| **push / pop**             | Di chuyển giữa các màn hình      |
| **go_router / auto_route** | Thư viện điều hướng hiện đại     |
| **Route Settings**         | Truyền dữ liệu giữa các màn hình |

---

## ⚙️ 4. State Management (Quản lý trạng thái)

| Thuật ngữ           | Mô tả                                                |
| ------------------- | ---------------------------------------------------- |
| **setState()**      | Cập nhật lại widget hiện tại                         |
| **Provider**        | Thư viện state management phổ biến, nhẹ              |
| **Riverpod**        | Phiên bản nâng cao hơn Provider                      |
| **Bloc / Cubit**    | Kiến trúc quản lý trạng thái theo luồng sự kiện      |
| **GetX**            | Thư viện quản lý state, routing, dependency đơn giản |
| **InheritedWidget** | Cách truyền dữ liệu từ tổ tiên đến widget con        |

---

## 🧬 5. Networking & Dữ Liệu

| Thuật ngữ             | Mô tả                                           |
| --------------------- | ----------------------------------------------- |
| **http**              | Gọi API đơn giản                                |
| **dio**               | Thư viện HTTP nâng cao (interceptor, cancel...) |
| **json_serializable** | Tự động tạo model từ JSON                       |
| **sqflite**           | Cơ sở dữ liệu SQLite nội bộ                     |
| **Hive**              | DB NoSQL nhanh, nhẹ, không cần native binding   |
| **SharedPreferences** | Lưu key-value đơn giản                          |

---

## 🧪 6. Kiểm thử & Debug

| Thuật ngữ             | Mô tả                                       |
| --------------------- | ------------------------------------------- |
| **Widget Test**       | Test UI nhỏ                                 |
| **Unit Test**         | Kiểm tra logic thuần                        |
| **Integration Test**  | Test tương tác người dùng & nhiều màn hình  |
| **flutter_test**      | Package test mặc định của Flutter           |
| **DevTools**          | Bộ công cụ debug, inspect memory, layout... |
| **Flutter Inspector** | Xem cấu trúc cây widget trực tiếp           |

---

## 🚀 7. Build & Phát Hành

| Thuật ngữ                             | Mô tả                                |
| ------------------------------------- | ------------------------------------ |
| **APK / AAB / IPA**                   | File build Android/iOS               |
| **Flutter Build**                     | Lệnh build ứng dụng                  |
| **pubspec.yaml**                      | Tập tin quản lý thư viện và cấu hình |
| **Code Obfuscation**                  | Làm rối mã để tránh bị dịch ngược    |
| **App Signing**                       | Ký ứng dụng Android/iOS để phát hành |
| **CI/CD (Codemagic, GitHub Actions)** | Tự động hóa build và deploy app      |

---

## 🎨 8. Animation & Hiệu ứng

| Thuật ngữ                               | Mô tả                                |
| --------------------------------------- | ------------------------------------ |
| **AnimatedContainer / AnimatedOpacity** | Các widget hỗ trợ animation đơn giản |
| **Tween / AnimationController**         | Tạo animation tuỳ chỉnh              |
| **Hero Animation**                      | Hiệu ứng chuyển cảnh mượt mà         |
| **Lottie**                              | Animation JSON động                  |
| **Rive**                                | Công cụ thiết kế animation tương tác |

---

## 🧠 Khái niệm Kỹ thuật Quan trọng

| Thuật ngữ                          | Mô tả                                                        |
| ---------------------------------- | ------------------------------------------------------------ |
| **Widget Tree**                    | Cấu trúc cây của các widget trong app                        |
| **Build Phase**                    | Giai đoạn build lại UI                                       |
| **Lifecycle (initState, dispose)** | Vòng đời của StatefulWidget                                  |
| **RenderObject**                   | Lớp cơ bản tạo layout & vẽ UI                                |
| **Keys**                           | Xác định widget duy nhất, tránh mất trạng thái khi build lại |

---

## 📘 Gợi ý sử dụng tài liệu

- ✅ Tài liệu học Flutter từ cơ bản đến nâng cao
- ✅ Tài liệu onboard cho team mobile
- ✅ Tích hợp vào wiki dự án hoặc file README

---

> Nếu bạn cần thêm bản PDF hoặc sơ đồ Mindmap cho nội dung này, hãy yêu cầu!
