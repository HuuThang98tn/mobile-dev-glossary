# 🚀 Thuật Ngữ Chuyên Sâu Trong Flutter

Tài liệu này tổng hợp các thuật ngữ chuyên sâu trong phát triển ứng dụng Flutter. Tập trung vào hiệu suất, kiến trúc, rendering, isolate, và tương tác native để giúp bạn làm chủ Flutter ở cấp độ sản phẩm lớn.

---

## 🧠 1. Rendering Engine & UI Pipeline

| Thuật ngữ                                    | Mô tả                                                            |
| -------------------------------------------- | ---------------------------------------------------------------- |
| **Skia**                                     | Engine đồ họa mã nguồn mở mà Flutter sử dụng để vẽ giao diện     |
| **Layer Tree**                               | Cấu trúc trung gian đại diện UI trước khi vẽ                     |
| **RenderObject**                             | Thành phần thấp cấp quyết định layout & paint trong Flutter      |
| **Compositing**                              | Kết hợp các layer để hiển thị hiệu ứng và hiệu suất cao          |
| **RepaintBoundary**                          | Ngăn việc repaint không cần thiết bằng cách cô lập vùng render   |
| **Widget Tree / Element Tree / Render Tree** | Ba tầng cấu trúc UI: UI mô tả, cấu trúc runtime, và logic layout |

---

## 🧵 2. Isolate & Concurrency

| Thuật ngữ                  | Mô tả                                                                 |
| -------------------------- | --------------------------------------------------------------------- |
| **Isolate**                | Flutter không có thread truyền thống, dùng isolate để xử lý song song |
| **Event Loop**             | Cơ chế xử lý bất đồng bộ của Dart (giống JavaScript)                  |
| **Microtask Queue**        | Hàng đợi ưu tiên cao hơn event queue trong Dart                       |
| **compute()**              | Hàm tiện lợi để chạy hàm trong isolate mới                            |
| **ReceivePort / SendPort** | Giao tiếp giữa các isolate                                            |

---

## ⚙️ 3. Build System & Release

| Thuật ngữ                                         | Mô tả                                              |
| ------------------------------------------------- | -------------------------------------------------- |
| **Flutter Build Modes (debug, profile, release)** | Các chế độ build ứng dụng Flutter                  |
| **AOT (Ahead Of Time)**                           | Biên dịch mã Dart thành native khi release         |
| **JIT (Just In Time)**                            | Biên dịch tại runtime (debug mode) giúp hot reload |
| **flutter build apk / ios / web**                 | Lệnh build tương ứng cho từng nền tảng             |
| **obfuscate**                                     | Làm rối mã Dart khi build để tăng bảo mật          |

---

## 🔐 4. Tương tác Native & Bảo mật

| Thuật ngữ                                              | Mô tả                                                |
| ------------------------------------------------------ | ---------------------------------------------------- |
| **Platform Channel**                                   | Giao tiếp giữa Flutter (Dart) và native (Java/Swift) |
| **MethodChannel / EventChannel / BasicMessageChannel** | Các loại kênh giao tiếp trong Flutter                |
| **FFI (Foreign Function Interface)**                   | Gọi hàm native C/C++ từ Dart                         |
| **PlatformView**                                       | Hiển thị native view trong Flutter UI                |
| **Secure Storage**                                     | Lưu trữ dữ liệu nhạy cảm (keychain, keystore)        |

---

## 🧪 5. Debug, Logging & Testing

| Thuật ngữ                           | Mô tả                                                         |
| ----------------------------------- | ------------------------------------------------------------- |
| **Flutter DevTools**                | Bộ công cụ debug chính thức (timeline, memory, UI inspect...) |
| **Widget Inspector**                | Kiểm tra cấu trúc widget đang hiển thị                        |
| **assert()**                        | Dùng kiểm tra điều kiện khi debug                             |
| **integration_test / flutter_test** | Thư viện test tích hợp và đơn vị của Flutter                  |
| **Golden Test**                     | So sánh ảnh chụp giao diện (snapshot test)                    |

---

## 🎯 6. Quản lý State & Hiệu suất

| Thuật ngữ                              | Mô tả                                           |
| -------------------------------------- | ----------------------------------------------- |
| **StatefulWidget / StatelessWidget**   | Hai dạng widget quản lý trạng thái UI           |
| **InheritedWidget**                    | Truyền dữ liệu xuống cây widget hiệu quả        |
| **Provider / Riverpod / Bloc / Cubit** | Các thư viện quản lý state phổ biến             |
| **ChangeNotifier**                     | Cách đơn giản để notify thay đổi trong provider |
| **Selector / Consumer**                | Tối ưu hóa rebuild trong Provider               |
| **Rebuild / Widget Lifecycle**         | Kiểm soát vòng đời và tránh render thừa         |

---

## 📚 Gợi ý sử dụng

- ✅ Dành cho lập trình viên Flutter đã qua giai đoạn học cơ bản
- ✅ Làm tài liệu nội bộ cho team làm Flutter production
- ✅ Sử dụng làm checklist tối ưu hiệu suất & maintain code lớn

> Nếu bạn muốn xuất PDF, sơ đồ mindmap hoặc template trình bày đẹp hơn, chỉ cần yêu cầu!
