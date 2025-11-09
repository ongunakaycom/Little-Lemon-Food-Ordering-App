# 🍋 Little Lemon – iOS Food Ordering App

**Little Lemon** is an elegant Swift-based iOS application for a fictional Mediterranean restaurant. It showcases **SwiftUI**, **CoreData** for persistence, and follows the **MVVM** architectural pattern while adhering to a clean and consistent UI/UX based on provided wireframes and style guides.

---

## 🧱 Tech Stack

| Layer        | Technology                             |
| ------------ | -------------------------------------- |
| Language     | Swift                                  |
| UI Framework | SwiftUI                                |
| Architecture | MVVM                                   |
| Persistence  | CoreData                               |
| IDE          | Xcode                                  |
| Assets       | Provided by Little Lemon design system |
| Platform     | iOS                                    |

---

## 🎨 Design & UX

The app is built to match the provided **wireframes** and **style guides**:

* **Style Guides**: `PG_LittleLemon_StyleGuide.pdf`, `my-style-guide.pdf`
* **Wireframes**: `my-wireframe.pdf`, `Canvas_Wireframe.fig`, `Canvas_Wireframe_Final.fig`

Assets like food images, logos, and placeholders are stored in the `Little Lemon App Assets/` folder and integrated into `Assets.xcassets`.

---

## 🔐 Architecture

The app follows **MVVM (Model-View-ViewModel)**:

* **Models** – Represent menu items and lists.
* **ViewModels** – Handle business logic and CoreData operations.
* **Views** – SwiftUI screens such as `Home`, `Menu`, `DetailItem`, `Hero`, `UserProfile`, and `Onboarding`.

---

## 🧪 Features

✅ Onboarding screen with persistent user profile
✅ Home and Menu screens with local image assets
✅ Detail item views
✅ CoreData integration for persistent state
✅ Profile page with image placeholder and static info
✅ Style consistency with brand guidelines

---

## 📁 Project Structure

```
LittleLemonApp/
├── LittleLemonApp/
│   ├── Assets.xcassets/          # App icons, images
│   ├── CoreData/                 # Persistence and data models
│   ├── Models/                   # MenuItem and MenuList
│   ├── ViewModels/               # Business logic and CoreData operations
│   ├── Views/                    # SwiftUI screens and components
│   └── LittleLemonApp.swift      # App entry point
└── LittleLemonApp.xcodeproj/     # Xcode project
```

---

## 🖥 Local Setup

### Requirements

* Xcode 14+
* macOS Monterey or newer
* Swift 5.7+

### Run the App

```bash
# Open project in Xcode
open LittleLemonApp.xcodeproj
```

* Use an **iOS Simulator** or real device.
* The app builds and runs without additional setup.

---

## 📦 CoreData

* Uses `ExampleDatabase.xcdatamodeld` for menu selections and user info.
* `Persistence.swift` sets up the CoreData stack.
* `FetchedObjects.swift` provides reactive data wrappers for SwiftUI.

---

## 🧪 Testing & Linting

* Manual testing via Xcode interface.
* Automated tests can be added with **XCTest**.

---

<<<<<<< Updated upstream
## About Me

I'm Ongun Akay, a Senior Full-Stack Developer with expertise across various technologies.

- 👀 I specialize in full-stack development with extensive experience in frontend and backend technologies.
- 🌱 Currently, I'm sharpening my skills in advanced concepts of web development.
- 💞️ I’m always open to exciting collaborations and projects that challenge my abilities.
- 📫 You can reach me at [info@ongunakay.com](mailto:info@ongunakay.com).
=======
## 📬 About Me

I'm Ongun Akay, a Senior Full-Stack Developer with expertise across various technologies.

* 👀 Specializes in full-stack development across frontend and backend technologies.
* 🌱 Actively exploring advanced web development concepts.
* 💞️ Open to collaborations and challenging projects.
* 📫 Reach me at: [info@ongunakay.com](mailto:info@ongunakay.com)
>>>>>>> Stashed changes

---

## 📄 License

MIT License – See [`LICENSE`](./LICENSE)
