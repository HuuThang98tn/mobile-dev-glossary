# 🚀 Thuật Ngữ Chuyên Sâu Trong Mobile App

Tài liệu này dành cho các lập trình viên phát triển ứng dụng di động chuyên sâu, bao gồm Android, iOS, và cross-platform. Nội dung tập trung vào hiệu suất, bảo mật, tối ưu build, đa luồng và kiến trúc hệ thống lớn.

---

## 🧠 1. Hiệu suất & Đa luồng (Performance & Threading)

| Thuật ngữ                             | Mô tả                                           |
| ------------------------------------- | ----------------------------------------------- |
| **Main Thread / UI Thread**           | Luồng chính xử lý giao diện người dùng          |
| **Background Thread / Worker Thread** | Dùng để xử lý các tác vụ nặng, tránh làm lag UI |
| **ANR (Application Not Responding)**  | Lỗi do chặn luồng UI quá lâu (Android)          |
| **Jank / Frame Drop**                 | Khung hình bị bỏ qua làm app giật (FPS < 60)    |
| **FPS (Frames Per Second)**           | Tốc độ khung hình – càng cao càng mượt          |
| **Thread Pool / Executor**            | Quản lý nhiều luồng hiệu quả (Android)          |
| **GCD (Grand Central Dispatch)**      | Cơ chế quản lý đa luồng (iOS)                   |

---

## 📦 2. Bộ nhớ & Tối ưu hóa (Memory Management)

| Thuật ngữ                              | Mô tả                                              |
| -------------------------------------- | -------------------------------------------------- |
| **Memory Leak**                        | Bộ nhớ bị chiếm mãi không được giải phóng          |
| **GC (Garbage Collection)**            | Hệ thống tự dọn dẹp bộ nhớ không dùng (Android)    |
| **ARC (Automatic Reference Counting)** | iOS tự đếm số tham chiếu để giải phóng bộ nhớ      |
| **OOM (Out of Memory)**                | App bị crash do hết bộ nhớ                         |
| **Memory Profiler**                    | Công cụ kiểm tra bộ nhớ bị rò rỉ                   |
| **Retain Cycle**                       | 2 object giữ nhau khiến không thể giải phóng (iOS) |

---

## 🔧 3. Build System & CI/CD

| Thuật ngữ                | Mô tả                                              |
| ------------------------ | -------------------------------------------------- |
| **Gradle / Xcodebuild**  | Công cụ build Android/iOS                          |
| **APK / AAB / IPA**      | File cài đặt Android/iOS                           |
| **Proguard / R8**        | Làm rối và tối ưu bytecode Android                 |
| **Bitcode**              | Intermediate code của iOS cho tối ưu build         |
| **CI/CD**                | Tự động hoá build, test, phát hành                 |
| **Code Signing**         | Ký ứng dụng để đảm bảo tính toàn vẹn               |
| **Provisioning Profile** | Hồ sơ cấp quyền để chạy app trên thiết bị iOS thật |

---

## 🔐 4. Bảo mật & Xác thực

| Thuật ngữ                                           | Mô tả                                                   |
| --------------------------------------------------- | ------------------------------------------------------- |
| **Secure Storage**                                  | Lưu trữ an toàn thông tin nhạy cảm (Keychain, Keystore) |
| **JWT / OAuth2**                                    | Cơ chế xác thực phổ biến                                |
| **Biometric Auth**                                  | Xác thực sinh trắc (vân tay, khuôn mặt)                 |
| **Certificate Pinning**                             | Ràng buộc kết nối HTTPS với chứng chỉ xác thực          |
| **Encrypted SharedPreferences / Realm / SQLCipher** | Lưu trữ dữ liệu mã hóa trong thiết bị                   |
| **Root / Jailbreak Detection**                      | Kiểm tra thiết bị đã bị can thiệp hệ thống              |

---

## 🌐 5. Giao tiếp mạng & đồng bộ dữ liệu

| Thuật ngữ                                         | Mô tả                               |
| ------------------------------------------------- | ----------------------------------- |
| **REST / GraphQL**                                | Các kiểu API phổ biến               |
| **WebSocket**                                     | Kết nối 2 chiều liên tục với server |
| **Caching Layer**                                 | Lưu trữ tạm dữ liệu để giảm gọi API |
| **Sync Adapter / Background Fetch / WorkManager** | Đồng bộ hóa dữ liệu tự động         |
| **Rate Limiting / Retry Strategy**                | Hạn chế & xử lý lỗi mạng hiệu quả   |

---

## 🎨 6. Rendering & UI nâng cao

| Thuật ngữ                      | Mô tả                                      |
| ------------------------------ | ------------------------------------------ |
| **Skia**                       | Engine vẽ đồ hoạ cho Android, Flutter      |
| **Core Animation / CA Layers** | Engine đồ họa của iOS                      |
| **Canvas / Custom Drawing**    | Vẽ UI tùy biến thủ công                    |
| **Layout Invalidation**        | Cơ chế hệ thống UI vẽ lại khi có thay đổi  |
| **Double Buffering**           | Tránh hiện tượng xé hình khi vẽ khung hình |

---

## 🧪 7. Testing & Debug

| Thuật ngữ                               | Mô tả                                  |
| --------------------------------------- | -------------------------------------- |
| **Unit Test**                           | Kiểm thử logic nhỏ                     |
| **UI Test / Espresso / XCTest / Detox** | Mô phỏng hành vi người dùng            |
| **Mocking / Stubbing**                  | Giả lập response hoặc module           |
| **Crashlytics / Sentry**                | Ghi log khi app crash ngoài production |
| **Test Coverage**                       | Tỉ lệ code được kiểm thử               |
| **ADB / LLDB**                          | Gỡ lỗi dòng lệnh trên Android/iOS      |

---

## 📱 8. Cross-platform nâng cao

| Thuật ngữ                              | Mô tả                               |
| -------------------------------------- | ----------------------------------- |
| **React Native / Flutter**             | Framework viết app đa nền tảng      |
| **Bridge / JSI / FFI**                 | Cầu nối giữa code JS/Dart và native |
| **Code Sharing**                       | Tái sử dụng logic giữa các nền tảng |
| **Platform Channels / Method Channel** | Giao tiếp native của Flutter        |
| **Hermes / Dart VM / TurboModules**    | Runtime engine cho cross-platform   |

---
