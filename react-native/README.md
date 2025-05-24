# 📱 Tổng Hợp Thuật Ngữ Trong React Native

Tài liệu này tổng hợp các thuật ngữ quan trọng trong phát triển ứng dụng React Native, được chia theo nhóm chức năng để dễ học, dễ tra cứu và sử dụng trong dự án hoặc đào tạo nội bộ.

---

## 📦 1. Cốt lõi của React Native

| Thuật ngữ          | Mô tả                                                           |
| ------------------ | --------------------------------------------------------------- |
| **React Native**   | Framework để xây app mobile bằng JavaScript (React)             |
| **Bridge**         | Cầu nối giữa JS và native code (Java/Kotlin, Objective-C/Swift) |
| **JS Thread**      | Luồng xử lý JavaScript trong React Native                       |
| **Native Modules** | Mô-đun native được viết bằng Java/Swift để mở rộng khả năng RN  |
| **Babel**          | Bộ chuyển đổi ES6+ thành JS tương thích với thiết bị            |
| **Metro Bundler**  | Công cụ build, bundling JS code cho RN                          |

---

## 🧩 2. Thành phần & Giao diện (UI)

| Thuật ngữ                        | Mô tả                                                        |
| -------------------------------- | ------------------------------------------------------------ |
| **View**                         | Thành phần cơ bản dùng để xây layout (như `<div>` trong web) |
| **Text**                         | Dùng để hiển thị chữ                                         |
| **Image**                        | Hiển thị hình ảnh                                            |
| **ScrollView**                   | Cuộn toàn bộ nội dung con                                    |
| **FlatList / SectionList**       | Hiển thị danh sách hiệu suất cao                             |
| **TouchableOpacity / Pressable** | Thành phần có thể tương tác, giống nút                       |
| **SafeAreaView**                 | Đảm bảo nội dung không bị che (tai thỏ, notch)               |
| **StyleSheet**                   | API định dạng kiểu (CSS-like)                                |
| **Flexbox**                      | Cách sắp xếp layout trong RN                                 |

---

## 🔁 3. Navigation (Điều hướng)

| Thuật ngữ                          | Mô tả                                           |
| ---------------------------------- | ----------------------------------------------- |
| **React Navigation**               | Thư viện điều hướng phổ biến trong RN           |
| **Stack Navigator**                | Mỗi màn hình được push lên stack                |
| **Bottom Tabs / Drawer Navigator** | Điều hướng dạng tab hoặc menu bên               |
| **Params / Route**                 | Tham số truyền giữa các màn hình                |
| **Navigation Container**           | Bao toàn bộ hệ thống điều hướng                 |
| **useNavigation / useRoute**       | Hook điều hướng trong RN (React Navigation v5+) |

---

## ⚙️ 4. State & Lifecycle

| Thuật ngữ                    | Mô tả                                       |
| ---------------------------- | ------------------------------------------- |
| **useState**                 | Hook quản lý state đơn giản                 |
| **useEffect**                | Hook xử lý lifecycle (componentDidMount...) |
| **Context API**              | Truyền dữ liệu global qua component tree    |
| **Redux / Zustand / Recoil** | Quản lý state toàn app                      |
| **useCallback / useMemo**    | Tối ưu hiệu suất re-render                  |

---

## 🧬 5. Networking & API

| Thuật ngữ                                | Mô tả                                             |
| ---------------------------------------- | ------------------------------------------------- |
| **Axios / Fetch**                        | Dùng gọi API REST                                 |
| **AsyncStorage**                         | Lưu trữ local dạng key-value (giống localStorage) |
| **Realm / SQLite**                       | Cơ sở dữ liệu local trên thiết bị                 |
| **Query / Mutation / SWR / React Query** | Thư viện quản lý fetch dữ liệu hiện đại           |

---

## 🧪 6. Kiểm thử & Debug

| Thuật ngữ                        | Mô tả                                                       |
| -------------------------------- | ----------------------------------------------------------- |
| **Jest**                         | Framework unit test cho React Native                        |
| **React Native Testing Library** | Test UI logic React Native                                  |
| **Detox**                        | E2E test (mô phỏng tương tác người dùng)                    |
| **Flipper**                      | Tool debug chính thức cho RN (giao diện, Redux, Network...) |
| **Remote Debugging**             | Chạy JS code trong Chrome                                   |
| **Fast Refresh**                 | Reload UI khi thay đổi code JS nhanh                        |

---

## 🚀 7. Build & Phát hành

| Thuật ngữ                | Mô tả                                            |
| ------------------------ | ------------------------------------------------ |
| **APK / AAB / IPA**      | File build Android/iOS                           |
| **Gradle**               | Build system Android                             |
| **Xcode**                | IDE và build tool của iOS                        |
| **Hermes**               | JS engine nhẹ, tối ưu hiệu suất cho RN           |
| **EAS Build / Expo CLI** | Công cụ build đám mây Expo                       |
| **Code Push**            | Cập nhật JS mà không cần phát hành lại lên store |
| **App Signing**          | Ký ứng dụng để phát hành chính thức              |

---

## 🎨 8. Thư viện & Hệ sinh thái

| Thư viện                         | Mô tả                                   |
| -------------------------------- | --------------------------------------- |
| **React Native Reanimated**      | Xử lý animation mượt và native          |
| **React Native Gesture Handler** | Quản lý gesture chạm hiệu suất cao      |
| **Lottie**                       | Hiển thị animation JSON động            |
| **react-native-svg**             | Vẽ SVG trong app                        |
| **react-native-paper**           | Bộ UI component theo Material Design    |
| **shadcn/ui-rn**                 | Bộ UI hiện đại (nếu dùng shadcn với RN) |

---

## 🧠 Các Khái Niệm Kỹ Thuật Quan Trọng

| Khái niệm                      | Mô tả                                                           |
| ------------------------------ | --------------------------------------------------------------- |
| **Bridging**                   | Giao tiếp giữa JavaScript và native code                        |
| **Threading**                  | Phân luồng xử lý trong RN (JS thread, UI thread, native thread) |
| **Re-render / Reconciliation** | Cơ chế cập nhật lại giao diện khi state thay đổi                |
| **Virtual DOM**                | Cơ chế DOM ảo giúp React/RN render hiệu quả hơn                 |
| **Batched Updates**            | Gộp nhiều thay đổi state để giảm render                         |

---

## 📘 Gợi ý sử dụng tài liệu

- ✅ Làm **tài liệu onboarding** cho team React Native mới
- ✅ Dùng làm **checklist học React Native** từ cơ bản đến nâng cao
- ✅ Tích hợp vào **wiki nội bộ** hoặc README chính của dự án

---

# 🚀 Thuật Ngữ Chuyên Sâu Trong React Native

Tài liệu này dành cho các lập trình viên React Native đã có kinh nghiệm, giúp hiểu rõ cơ chế nội bộ, tối ưu hiệu suất, tương tác native và build hệ thống lớn.

---

## 🧠 1. Kiến trúc nội bộ (Core Architecture)

| Thuật ngữ                      | Mô tả                                                                                                |
| ------------------------------ | ---------------------------------------------------------------------------------------------------- |
| **JSI (JavaScript Interface)** | Cơ chế mới thay thế Bridge truyền thống, giúp gọi native function từ JS không cần JSON serialization |
| **Fabric**                     | Hệ thống rendering engine mới (tăng tốc rendering, async layout)                                     |
| **TurboModules**               | Thay thế cho NativeModules cũ, cho phép lazy load module native khi cần                              |
| **Shadow Tree**                | Cấu trúc trung gian biểu diễn UI được tính toán trước khi render thực tế                             |
| **Reconciler**                 | Cơ chế so sánh Virtual DOM và cập nhật UI khi state thay đổi                                         |
| **Renderer Threads**           | Bao gồm JS thread, UI thread, Native modules thread                                                  |
| **Scheduler**                  | Quản lý ưu tiên task trong JS thread để tránh UI bị lag                                              |

---

## 🔁 2. Hiệu suất & Tối ưu hoá

| Thuật ngữ                   | Mô tả                                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------------- |
| **Batched Updates**         | React Native tự động gom nhiều state update lại thành 1 lần re-render để tiết kiệm tài nguyên |
| **Offloading to Native**    | Di chuyển các tác vụ nặng như xử lý ảnh, video, animation sang native code                    |
| **Memoization**             | Tối ưu re-render qua React.memo, useMemo, useCallback                                         |
| **UI Blocking**             | Xảy ra khi JS thread bị chiếm dụng bởi tác vụ nặng (dẫn đến UI delay)                         |
| **FPS (Frames Per Second)** | Đơn vị đo độ mượt, mục tiêu ≥ 60 FPS                                                          |
| **InteractionManager**      | Đợi khi animation/UI hoàn thành mới chạy tác vụ JS để không làm giật hình                     |

---

## 🔐 3. Native Interop & Cầu nối

| Thuật ngữ                                  | Mô tả                                                    |
| ------------------------------------------ | -------------------------------------------------------- |
| **Native Modules**                         | Module được viết bằng Java/Kotlin hoặc Objective-C/Swift |
| **Bridging**                               | Cơ chế kết nối giữa JS và Native (cũ, bị thay bởi JSI)   |
| **Callbacks / Promises in Native Modules** | Truyền kết quả async giữa JS và native                   |
| **Headless JS**                            | Chạy code JS trong nền (background tasks)                |
| **AppRegistry**                            | Entry point đăng ký các components chính cho native side |

---

## 🧪 4. Testing & Debug Tools

| Thuật ngữ               | Mô tả                                                                 |
| ----------------------- | --------------------------------------------------------------------- |
| **Mock Native Modules** | Giả lập native module để test unit JS                                 |
| **Flipper Plugins**     | Mở rộng khả năng inspect Redux, mạng, DB...                           |
| **Hermes Debugger**     | Gỡ lỗi JS trực tiếp trong Hermes engine                               |
| **Console Polyfill**    | Các hàm log như console.log được thay đổi để hoạt động trong thiết bị |

---

## 🧰 5. Build System & Release

| Thuật ngữ            | Mô tả                                                               |
| -------------------- | ------------------------------------------------------------------- |
| **Hermes**           | JS Engine nhẹ, hiệu suất cao cho Android & iOS                      |
| **Multidex**         | Khi số method vượt quá 64K, Android cần bật tính năng này           |
| **Proguard**         | Làm rối & tối ưu code khi release Android build                     |
| **Bundle Splitting** | Tách code theo từng màn hình/module để giảm dung lượng initial load |
| **Inline Requires**  | Kỹ thuật lazy load module trong Metro bundler để giảm startup time  |

---

## 📚 6. Phát triển Module/Library riêng

| Thuật ngữ                           | Mô tả                                                              |
| ----------------------------------- | ------------------------------------------------------------------ |
| **react-native-builder-bob**        | CLI tool tạo boilerplate cho native module/package mới             |
| **Monorepo (Lerna, Nx)**            | Quản lý nhiều package trong 1 repo (tốt khi bạn tự phát triển lib) |
| **Codegen (RCT_EXPORT_MODULE)**     | Tự động generate bridge code khi viết native module                |
| **Typed Native Modules (TS + JSI)** | Kết hợp TypeScript với JSI để native module có typed interface     |

---

## 🌐 7. Cross-platform nâng cao

| Thuật ngữ                                              | Mô tả                                                  |
| ------------------------------------------------------ | ------------------------------------------------------ |
| **Platform-specific Code**                             | Dùng .ios.js / .android.js để viết riêng từng nền tảng |
| **Dynamic Import (Platform.OS)**                       | Viết logic chọn module theo nền tảng tại runtime       |
| **Linking / Permissions**                              | Giao tiếp với deep link, hệ thống quyền                |
| **Push Notification (APNs, FCM)**                      | Tích hợp thông báo với native SDK                      |
| **Background Task / Headless JS / Foreground Service** | Xử lý tác vụ chạy trong nền Android/iOS                |

---
