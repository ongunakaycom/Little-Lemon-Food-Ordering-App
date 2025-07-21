# 🍋 Little Lemon – iOS Food Ordering App

**Little Lemon** is an elegant Swift-based iOS app designed for a fictional Mediterranean restaurant. This project demonstrates UI building with **SwiftUI**, data persistence with **CoreData**, MVVM architecture, and a refined UI/UX based on provided wireframes and style guides.

---

## 🧱 Stack Overview

| Layer         | Technology                  |
|--------------|------------------------------|
| Language      | Swift                        |
| UI Framework  | SwiftUI                     |
| State Mgmt    | MVVM Architecture            |
| Persistence   | CoreData                     |
| IDE           | Xcode                        |
| Assets        | Provided by Little Lemon design system |
| Platform      | iOS                          |

---

## 🎨 UX & Design

The app's interface is designed to match the provided style guides and wireframes:

- **Style Guides**: `PG_LittleLemon_StyleGuide.pdf`, `my-style-guide.pdf`
- **Wireframes**: `my-wireframe.pdf`, `Canvas_Wireframe.fig`, `Canvas_Wireframe_Final.fig`

Visual assets like food items, logos, and placeholders are stored in the `Little Lemon App Assets/` and embedded into `Assets.xcassets`.

---

## 🔐 Architecture

The app follows the **MVVM (Model-View-ViewModel)** pattern:

- **Models**: Represent menu items and lists.
- **ViewModels**: Handle business logic and CoreData operations.
- **Views**: SwiftUI screens like `Home`, `Menu`, `Hero`, `UserProfile`, and `Onboarding`.

---

## 🧪 Features

✅ Onboarding screen with persistent user profile  
✅ Home and Menu screens with local image assets  
✅ Detail item views  
✅ CoreData integration for persistent state  
✅ Profile page with image placeholder and static info  
✅ Style consistency per brand guidelines

---

## 📁 Directory Structure

```
LittleLemonApp/
├── LittleLemonApp/
│   ├── Assets.xcassets/         # App icons, images
│   ├── CoreData/                # Persistence and data models
│   ├── Models/                  # MenuItem and MenuList
│   ├── ViewModels/              # ViewModel logic
│   ├── Views/                   # SwiftUI components
│   └── LittleLemonApp.swift     # App entry point
└── LittleLemonApp.xcodeproj/    # Xcode project
```

---

## 🧰 Local Development Setup

### 🖥 Requirements

- Xcode 14+  
- macOS Monterey or newer  
- Swift 5.7+

### 🚀 Run the App

```bash
# Open project
open LittleLemonApp.xcodeproj
```

- Use an **iOS Simulator** or real device.
- The app builds and runs with no additional setup.

---

## 📦 CoreData

- Uses `ExampleDatabase.xcdatamodeld` to persist menu selections and user info.
- `Persistence.swift` handles setup and context management.
- `FetchedObjects.swift` provides wrapper logic for reactive views.

---

## 🧪 Linting & Testing

Manual testing via Xcode interface.

> ℹ️ Note: Automated UI/unit tests can be added using XCTest framework.

---

## 📬 Author

I'm Ongun Akay, a Senior Full-Stack Developer with expertise across various technologies.

About Me
👀 I specialize in full-stack development with extensive experience in frontend and backend technologies.
🌱 Currently, I'm sharpening my skills in advanced concepts of web development.
💞️ I’m always open to exciting collaborations and projects that challenge my abilities.
📫 You can reach me at info@ongunakay.com.
---

## 📄 License

MIT License – See [`LICENSE`](./LICENSE)