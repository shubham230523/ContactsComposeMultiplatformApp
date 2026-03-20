# ContactsComposeMultiplatformApp 📱

A professional cross-platform contact management application built using **Compose Multiplatform (CMP)** and **Kotlin Multiplatform (KMM)**. This project demonstrates a unified codebase for both Android and iOS, implementing a scalable MVI architecture and native integrations.

---

## 🌟 Features

* **Cross-Platform UI:** Shared UI components across Android and iOS using Compose Multiplatform.
* **MVI Architecture:** Unidirectional data flow for predictable state management.
* **Full CRUD Logic:** Create, view, edit, and delete contacts with a local database.
* **Image Handling:** Native photo picking and storage implementation for both platforms.
* **Material 3:** Modern design system with:
    * **Dynamic Theming:** Adapts to user wallpaper on Android.
    * **Dark Mode:** Full support for system-wide dark/light themes.
* **Persistent Storage:** Robust local data handling using **SQLDelight**.

---

## 🛠 Tech Stack

| Category | Technology |
| :--- | :--- |
| **Language** | Kotlin |
| **Framework** | Compose Multiplatform (CMP) |
| **Architecture** | MVI (Model-View-Intent) |
| **Database** | SQLDelight |
| **DI** | Manual Dependency Injection |
| **Design** | Material 3 |

---

## 🏗 Project Structure

```text
.
├── composeApp
│   ├── commonMain      # Shared logic, UI (Composables), and MVI components
│   ├── androidMain     # Android-specific implementations (DB drivers, UI wrappers)
│   └── iosMain         # iOS-specific implementations (entry point, DB drivers)
└── iosApp              # Swift project wrapper for iOS
