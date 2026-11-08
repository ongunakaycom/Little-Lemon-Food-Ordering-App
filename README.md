# 🍋 Little Lemon – iOS Food Ordering App

![Swift](https://img.shields.io/badge/Swift-5.7-orange?logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-5.7-blue?logo=ios&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-14+-red?logo=xcode&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-15%2B-lightgray?logo=apple&logoColor=white)
![MVVM](https://img.shields.io/badge/MVVM-architecture-success?logo=react&logoColor=white)
![CoreData](https://img.shields.io/badge/CoreData-persistent-green?logo=database&logoColor=white)
![Combine](https://img.shields.io/badge/Combine-reactive-purple?logo=swift&logoColor=white)

**Little Lemon** is an elegant SwiftUI iOS application for a fictional Mediterranean restaurant. Built as the capstone project for the **Meta iOS Developer Professional Certificate**, the app demonstrates modern iOS development practices including SwiftUI, CoreData for persistent storage, MVVM architecture, and Combine for reactive state management.

🌐 **[View the Portfolio Page](https://ongunakaycom.github.io/Little-Lemon-Food-Ordering-App/)**

---

## 📸 Screenshots

*(Note to author: Replace these placeholders with actual screenshots from your simulator. This is the most important step for a UI/UX portfolio!)*

| Onboarding | Home & Menu | Detail View | User Profile |
| :---: | :---: | :---: | :---: |
| ![Onboarding](docs/assets/onboarding.png) | ![Home](docs/assets/home.png) | ![Detail](docs/assets/detail.png) | ![Profile](docs/assets/profile.png) |

---

## 🛠 Technologies Used

| Layer | Technology |
| :--- | :--- |
| **Language** | Swift 5.7+ |
| **UI Framework** | SwiftUI |
| **Architecture** | MVVM (Model-View-ViewModel) |
| **Persistence** | CoreData |
| **Networking** | URLSession + Combine |
| **Security** | CryptoKit (AES.GCM for email encryption) |
| **IDE** | Xcode 14+ |
| **Platform** | iOS (iPhone & iPad) |

---

## ✨ Key Features

*   **Onboarding & Authentication:** Secure user registration with input validation. Persists login state seamlessly via `UserDefaults`.
*   **Dynamic Menu:** Fetches menu JSON from a remote API. Features category toggles (starters, mains, desserts, drinks), real-time search, and filtering.
*   **Detail Views:** Beautiful full-screen dish presentations using `AsyncImage` for remote image loading.
*   **User Profile:** Allows users to view and edit their details. Includes local encryption using `CryptoKit` and toggle-based user preferences.
*   **Robust Persistence:** Fully integrated `CoreData` stack. Includes a reactive `FetchedObjects` wrapper for automatic SwiftUI updates and a `clear()` method for efficient data refreshing.

---

## 📁 Project Architecture

The project follows a clean **MVVM** architecture to ensure separation of concerns and maintainable code.

```text
LittleLemonApp/
├── LittleLemonApp/
│   ├── Assets.xcassets/              # App icons, colors, and images
│   ├── CoreData/                     # Persistence stack
│   │   ├── ExampleDatabase.xcdatamodeld
│   │   ├── Persistence.swift
│   │   └── FetchedObjects.swift
│   ├── Models/                       # Data models (MenuItem, MenuList)
│   ├── ViewModels/                   # Business logic & state management
│   ├── Views/                        # SwiftUI screens & components
│   │   ├── Onboarding.swift
│   │   ├── Home.swift
│   │   ├── MainScreen.swift
│   │   ├── Menu.swift
│   │   ├── Hero.swift
│   │   ├── Header.swift
│   │   ├── DetailItem.swift
│   │   └── FoodItem.swift
│   └── LittleLemonApp.swift          # App entry point
└── LittleLemonApp.xcodeproj/         # Xcode project file
```

---

## 🚀 Getting Started

### Requirements
*   Xcode 14+ (or newer)
*   macOS Monterey (12+) or newer
*   Swift 5.7+

### Run the App Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ongunakaycom/Little-Lemon-Food-Ordering-App.git
   ```
2. **Open the project in Xcode:**
   ```bash
   open LittleLemonApp.xcodeproj
   ```
3. Select an iOS simulator (e.g., iPhone 15) or a connected physical device.
4. Press **`Cmd + R`** or click the "Play" button to build and run.
5. The app will launch on the **Onboarding Screen**. Enter user details and tap **Register** to proceed to the Home screen.

---

## 🧪 Quality & Testing

*   **Architecture:** Strict adherence to MVVM principles for testability.
*   **Code Quality:** Clean, well-documented Swift code following Apple's Human Interface Guidelines.
*   **Security:** Handled via native Apple frameworks (CryptoKit for data encryption).
*   **Continuous Integration:** GitHub Actions configured for automated deployment of the portfolio page.

*(Note: XCTest implementation is planned for future iterations to cover ViewModel logic and CoreData operations.)*

---

## 👤 Author

**Ongun Akay**
*Mobile Developer | iOS & SwiftUI Enthusiast*

*   **GitHub:** [@ongunakaycom](https://github.com/ongunakaycom)
*   **Portfolio:** [ongunakay.com](https://ongunakay.com)
*   **Email:** [info@ongunakay.com](mailto:info@ongunakay.com)

---

## 📄 License

This project is licensed under the **MIT License** – see the [`LICENSE`](./LICENSE) file for details.

---
*Built with ❤️ as part of the Meta iOS Developer Professional Certificate program.*