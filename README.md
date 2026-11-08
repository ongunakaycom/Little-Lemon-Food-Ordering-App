# 🍋 Little Lemon – iOS Food Ordering App

![Swift](https://img.shields.io/badge/Swift-5.7-orange?logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-5.7-blue?logo=ios&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-14+-red?logo=xcode&logoColor=white)
![iOS](https://img.shields.io/badge/iOS-15%2B-lightgray?logo=apple&logoColor=white)
![MVVM](https://img.shields.io/badge/MVVM-architecture-success?logo=react&logoColor=white)
![CoreData](https://img.shields.io/badge/CoreData-persistent-green?logo=database&logoColor=white)
![Combine](https://img.shields.io/badge/Combine-reactive-purple?logo=swift&logoColor=white)
![Meta](https://img.shields.io/badge/Meta-iOS%20Developer%20Certificate-1a73e8?logo=meta&logoColor=white)

**Little Lemon** is an elegant SwiftUI iOS application for a fictional Mediterranean restaurant, built as the capstone project for the **Meta iOS Developer Professional Certificate** on Coursera. The app demonstrates modern iOS development practices including SwiftUI, CoreData for persistent storage, MVVM architecture, and Combine for reactive state management.

> *This project was developed to showcase job-ready iOS development skills, including UI design, data persistence, networking, and clean architecture.*

## 🛠 Technologies

| Layer | Technology |
| --- | --- |
| **Language** | Swift 5.7+ |
| **UI Framework** | SwiftUI |
| **Architecture** | MVVM (Model-View-ViewModel) |
| **Persistence** | CoreData |
| **Networking** | URLSession + Combine |
| **IDE** | Xcode 14+ |
| **Platform** | iOS (iPhone & iPad) |

---

## ✨ Key Features

- **Onboarding** – User registration with input validation; persists login state via `UserDefaults`.
- **Home & Menu** – Header with profile avatar, hero section, category toggles (starters, mains, desserts, drinks), search/filtering/sorting, and a scrollable dish list from CoreData.
- **Detail Item** – Full-screen dish view with `AsyncImage`, title, description, and price.
- **User Profile** – Display/edit personal details; email encryption via `AES.GCM`; toggle settings; Save/Discard with persistent storage.
- **CoreData Persistence** – Persistent local storage; `clear()` method for re-fetching; `FetchedObjects` reactive wrapper.
- **Networking** – Fetches menu JSON from GitHub API; decodes into `MenuItem` structs; maps to CoreData entities.

---

## 📁 Project Structure

```text
LittleLemonApp/
├── LittleLemonApp/
│   ├── Assets.xcassets/              # App icons, images, color sets
│   ├── CoreData/                     # Persistence stack & data models
│   │   ├── ExampleDatabase.xcdatamodeld
│   │   ├── Persistence.swift
│   │   └── FetchedObjects.swift
│   ├── Models/                       # Codable structs: MenuItem, MenuList
│   ├── ViewModels/                   # Business logic: ViewModel
│   ├── Views/                        # SwiftUI screens & components
│   │   ├── Onboarding.swift
│   │   ├── Home.swift
│   │   ├── MainScreen.swift
│   │   ├── Menu.swift
│   │   ├── Hero.swift
│   │   ├── Header.swift
│   │   ├── DetailItem.swift
│   │   └── FoodItem.swift
│   └── LittleLemonApp.swift
└── LittleLemonApp.xcodeproj/
```

---

## 🚀 Local Setup

### Requirements
- Xcode 14+ (or newer)
- macOS Monterey (12+) or newer
- Swift 5.7+

### Run the App

```bash
# 1. Clone the repository
git clone https://github.com/ongunakaycom/Little-Lemon-Food-Ordering-App.git

# 2. Open project in Xcode
open LittleLemonApp.xcodeproj
```

3. Select an iOS simulator (e.g., iPhone 15) or connect a physical device.
4. Press **Cmd+R** or click the "Play" button in Xcode to build and run.
5. The app launches on the **Onboarding Screen** – enter user details and tap **Register** to proceed to Home.

---

## 🗺 Roadmap

- [ ] Add XCTest unit tests for `ViewModel.validateUserInput()`
- [ ] Handle network errors gracefully in `MenuList.getMenuData()`
- [ ] Add dark mode support for all color assets
- [ ] Add search debounce (0.5s) for better performance
- [ ] Improve accessibility labels across all interactive elements
- [ ] Add iPad split-view support for `MainScreen` and `DetailItem`

---

## 👤 Author

**Ongun Akay** – Mobile Developer passionate about building clean, maintainable iOS applications.

- GitHub: [@ongunakaycom](https://github.com/ongunakaycom)
- Project: [Little-Lemon-Food-Ordering-App](https://github.com/ongunakaycom/Little-Lemon-Food-Ordering-App)
- Portfolio: [ongunakaycom.github.io](https://ongunakaycom.github.io/Little-Lemon-Food-Ordering-App/)
- Email: info@ongunakay.com

---

## 📄 License

This project is licensed under the **MIT License** – see the [`LICENSE`](./LICENSE) file for details.

---

*Built with ❤️ during the Meta iOS Developer Professional Certificate program on Coursera.*