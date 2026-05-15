<img width="200"  alt="5a692901-d117-47a2-9465-34317542ede3" src="https://github.com/user-attachments/assets/7b837d61-dc0a-44c3-9161-aeb12e03f22b" />
<img width="200" alt="b4582c4c-6f0f-4147-a78a-11339b593ded" src="https://github.com/user-attachments/assets/a3ed106c-a50f-4f45-986c-dc6f1fc6ada0" />
<img width="200" alt="2656098a-5c4f-4791-8502-937467d27e0b" src="https://github.com/user-attachments/assets/2d7d18d8-ef1d-4bc1-a9d7-822bbc495b98" />
<img width="200"  alt="28178f00-95ec-4dc2-ab13-1a29d434659f" src="https://github.com/user-attachments/assets/bfcf74a4-2011-430e-8926-7d1a410e6892" />
<img width="200"  alt="128b05fc-6c1b-42c9-b6e1-9bc7c985741f" src="https://github.com/user-attachments/assets/e0ac3df2-6663-4202-a614-b9044e43019e" />
<img width="200" alt="5e853cdd-7894-4098-b43d-5ce549a37005" src="https://github.com/user-attachments/assets/91fe3bbc-9836-49fb-98d7-319116e12f76" />


# TaskManager App 📝

Một ứng dụng quản lý công việc (Task Management) chuẩn production dành cho iOS, được xây dựng với **SwiftUI** và **SwiftData**. Ứng dụng hỗ trợ quản lý công việc toàn diện với kiến trúc Offline-first, giao diện trực quan và tuân thủ chặt chẽ các nguyên tắc Clean Code cùng mô hình MVVM.

Đây là bài tập thực hành **Lab 11**.

## 🚀 Tính năng nổi bật

* **CRUD Operations:** Tạo mới, xem chi tiết, chỉnh sửa và xóa công việc dễ dàng.
* **Database Persistence:** Lưu trữ dữ liệu cục bộ an toàn và mượt mà với SwiftData (iOS 17+).
* **Task Management:** 
  * Đánh dấu hoàn thành/chưa hoàn thành (Status Toggle).
  * Phân loại mức độ ưu tiên: Low, Medium, High (Task Priority).
  * Quản lý thời hạn công việc (Deadline Management).
* **Smart Filtering & Search:**
  * Tìm kiếm công việc theo tên (Search bar).
  * Lọc công việc theo trạng thái: All, Pending, Done (Segmented Control).
* **Dashboard & Statistics:** Thống kê tổng số task, task đã hoàn thành và task đang chờ xử lý.
* **UI/UX:** Hỗ trợ Dark Mode, thiết kế giao diện hiện đại với các component được tái sử dụng (Reusable Components).

## 🛠 Công nghệ & Kiến trúc

* **Nền tảng:** iOS 17.0+
* **Ngôn ngữ:** Swift
* **UI Framework:** SwiftUI
* **Database:** SwiftData
* **Kiến trúc:** MVVM (Model - View - ViewModel)

## 📂 Cấu trúc dự án

```text
TaskManager/
│
├── Models/
│   ├── TaskItem.swift          # Data model chính (SwiftData @Model)
│   └── TaskPriority.swift      # Enum định nghĩa mức độ ưu tiên
│
├── ViewModels/
│   └── TaskViewModel.swift     # Xử lý logic lọc, tìm kiếm và state quản lý UI
│
├── Views/
│   ├── TaskListView.swift      # Màn hình chính (Dashboard & List)
│   ├── TaskEditorView.swift    # Màn hình thêm mới công việc
│   ├── TaskDetailView.swift    # Màn hình xem và chỉnh sửa chi tiết
│   └── StatisticsView.swift    # Màn hình thống kê
│
├── Components/
│   ├── TaskCardView.swift      # Card hiển thị item công việc
│   ├── PriorityBadge.swift     # Label hiển thị mức độ ưu tiên
│   ├── StatusToggle.swift      # Nút check hoàn thành
│   └── EmptyTaskView.swift     # Giao diện khi không có dữ liệu
│
└── TaskManagerApp.swift        # Entry point & Cấu hình ModelContainer
```
