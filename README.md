# 🍋 Little Lemon – iOS Food Ordering App

**Little Lemon** is an elegant SwiftUI iOS application for a fictional Mediterranean restaurant, built as the capstone project for the Meta iOS Developer Professional Certificate program on Coursera. The app demonstrates modern iOS development practices including **SwiftUI**, **CoreData** for persistent storage, **MVVM** architecture, and **Combine** for reactive state management.

---

## 🧱 Tech Stack

| Layer | Technology |
| --- | --- |
| **Language** | Swift 5.7+ |
| **UI Framework** | SwiftUI |
| **Architecture** | MVVM (Model-View-ViewModel) |
| **Persistence** | CoreData |
| **Networking** | URLSession + Combine |
| **IDE** | Xcode 14+ |
| **Platform** | iOS (iPhone & iPad) |
| **Assets** | Provided by Little Lemon design system (PDF wireframes & style guides) |

---

## 🎨 Design

The app is meticulously built to match the provided **wireframes** and **style guides**:

- **Style Guides**: `PG_LittleLemon_StyleGuide.pdf`, `my-style-guide.pdf`, `PG_LittleLemon_StyleGuide.pdf`
- **Wireframes**: `my-wireframe.pdf`, `Canvas_Wireframe.fig`, `Canvas_Wireframe_Final.fig`

Assets like food images, logos, and placeholders are stored in the `Little Lemon App Assets/` folder and integrated into `Assets.xcassets`. The design system includes custom fonts (`Karla`, `Markazi Text`) and a consistent color palette.

---

## 🔐 Architecture

The app follows **MVVM** separation of concerns:

| Component | Responsibility |
| --- | --- |
| **Models** (`Models/`) | `MenuItem` & `MenuList` – Codable structs for JSON decoding; `Dish` – CoreData entity for persistent storage |
| **ViewModels** (`ViewModels/`) | `ViewModel` – Handles user input validation, CoreData operations, UserDefaults persistence, and encryption (`CryptoKit`) |
| **Views** (`Views/`) | SwiftUI screens: `Onboarding`, `Home`, `MainScreen`, `Menu`, `Hero`, `DetailItem`, `FoodItem`, `UserProfile` |

Key data flow: JSON menu data → `MenuList.getMenuData()` → CoreData `Dish` entities → `FetchedObjects` with predicate/sort → SwiftUI list views with filtering/toggling.

---

## ✨ Features

| Feature | Description |
| --- | --- |
| **Onboarding** | Collects user details (first name, last name, email, phone) with validation; persists login state via `UserDefaults`; navigates to Home on successful registration. |
| **Home & Menu** | Header with profile avatar; hero section with restaurant description; category toggles (starters, mains, desserts, drinks); search/filtering/sorting; scrollable dish list from CoreData. |
| **Detail Item** | Full-screen view with `AsyncImage`, title, description, price, and nutritional/descriptive text. |
| **User Profile** | Displays/edits user personal details; email encryption via `AES.GCM`; toggle settings for order statuses, password changes, special offers, newsletter; Save/Discard changes with persistent storage. |
| **CoreData Persistence** | Persistent local storage for menu items and user preferences; `clear()` method to reset data before re-fetching; `FetchedObjects` reactive wrapper for SwiftUI. |
| **Networking** | Fetches menu JSON from GitHub API (`https://raw.githubusercontent.com/Meta-Mobile-Developer-PC/Working-With-Data-API/main/menu.json`); decodes into `MenuItem` structs; maps to CoreData entities. |

---

## 📁 Project Structure

```
LittleLemonApp/
├── LittleLemonApp/                    # Xcode project folder
│   ├── Assets.xcassets/              # App icons, images, color sets
│   ├── CoreData/                     # Persistence stack & data models
│   │   ├── ExampleDatabase.xcdatamodeld
│   │   ├── Persistence.swift         # NSPersistentContainer setup
│   │   └── FetchedObjects.swift       # Reactive fetch wrapper
│   ├── Models/                       # Codable structs: MenuItem, MenuList
│   ├── ViewModels/                   # Business logic: ViewModel (validation, persistence, encryption)
│   ├── Views/                      # SwiftUI screens & components
│   │   ├── Onboarding.swift         # User registration flow
│   │   ├── Home.swift               # Entry point → MainScreen
│   │   ├── MainScreen.swift         # Header + Menu container
│   │   ├── Menu.swift               # Search, filters, category toggles, dish list
│   │   ├── Hero.swift               # Restaurant hero section
│   │   ├── Header.swift             # Top bar with profile avatar
│   │   ├── DetailItem.swift         # Single dish detail view
│   │   └── FoodItem.swift           # List row dish component
│   └── LittleLemonApp.swift        # App entry point
└── LittleLemonApp.xcodeproj/         # Xcode project file
```

---

## 🧪 Local Setup

### Requirements

- **Xcode 14+** (or newer)
- **macOS Monterey** (12+) or newer
- **Swift 5.7+**
- iOS Simulator (built-in with Xcode) or real iOS device

### Run the App

```bash
# Open project in Xcode
open LittleLemonApp.xcodeproj
```

1. Select an iOS simulator (e.g., iPhone 15, iPhone 15 Pro Max) or connect a physical device.
2. Press **Cmd+R** or click the "Play" button in Xcode to build and run.
3. The app launches on the **Onboarding Screen** – enter user details and tap **Register** to proceed to Home.

---

## 🗄 CoreData Details

- **Database**: `ExampleDatabase.xcdatamodeld` – contains `Dish` entity for menu storage.
- **PersistenceController**: Sets up the CoreData stack; `viewContext` is injected via `\.managedObjectContext` environment variable.
- **`clear()`**: Deletes all `Dish` entities from the persistent store (used before re-fetching JSON menu data).
- **`oneDish()`**: Convenience static helper that returns a sample `Dish` instance for SwiftUI previews.
- **Automatic merging**: `automaticallyMergesChangesFromParent = true` ensures UI stays in sync with background context changes.

---

## 🧪 Testing & Linting

- **Manual testing**: Full workflow verification via Xcode interface (Onboarding → Home → Menu → Detail → Profile).
- **Automated tests**: XCTest test cases can be added for `ViewModel` validation, CoreData operations, and UI interactions.
- **No formal CI setup** – manual builds in Xcode recommended for development workflow.

---

## 👤 About Me

I'm **Ongun Akay**, a mobile developer passionate about building clean, maintainable iOS applications. This project serves as my capstone portfolio piece for the Meta iOS Developer Professional Certificate, demonstrating:

- SwiftUI expertise and adaptive UI design
- CoreData persistence and data modeling best practices
- MVVM architecture with separated concerns
- JSON networking and data decoding
- Custom toggles, animations, and accessibility considerations

---

## 📄 License

This project is licensed under the **MIT License** – see the [`LICENSE`](./LICENSE) file for details.

---

## 🚀 GitHub Pages Deployment (Portfolio)

Since this is an **iOS native app** (Xcode/SwiftUI), it cannot be directly deployed to GitHub Pages as a running application. However, you can showcase it on GitHub Pages in these ways:

### Option 1: Project Documentation Site (Recommended)
Convert this README into a beautiful documentation site using [GitHub Pages](https://pages.github.com/) with:
- Minimal Mistakes, Just the Docs, or Docusaurus template
- Include screenshots (see screenshots section below)
- Add a "Download" link to the Xcode project
- Showcase Tech Stack, Features, and Setup instructions

### Option 2: Screenshots & GIF Gallery
1. Add app screenshots/GIFs to a `/assets` folder
2. Create a `index.html` that displays them in a gallery
3. Enable GitHub Pages on `main` branch / `/docs` folder
4. Link from your portfolio/README

### Option 3: SwiftUI Code Showcase
1. Create a separate `docs/` branch or folder
2. Host SwiftUI code snippets, animations, and explanations
3. Use GitHub Pages to render the markdown documentation

### How to Set Up GitHub Pages:

```bash
# 1. Add screenshots to the repo
# 2. Create a /docs folder or use the /(root) with index.html
# 3. In GitHub repo Settings > Pages:
#    - Source: Select "main branch /root" or "docs folder"
# 4. Your site will be published at https://<username>.github.io/<repo-name>/

# Example index.html for screenshot gallery:
/*
<!DOCTYPE html>
<html>
<head>
    <title>Little Lemon - iOS App Portfolio</title>
    <style>
        body { max-width: 800px; margin: 0 auto; padding: 20px; font-family: sans-serif; }
        .gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 10px; }
        .gallery img { max-width: 100%; height: auto; border-radius: 8px; }
    </style>
</head>
<body>
    <h1>🍋 Little Lemon iOS App</h1>
    <p>Food Ordering App built with SwiftUI, CoreData, and MVVM</p>
    <div class="gallery">
        <!-- Screenshots will be auto-inserted by GitHub -->
    </div>
    <hr>
    <p><a href="https://github.com/ongunakaycom/Little-Lemon-Food-Ordering-App">View Source on GitHub</a></p>
</body>
</html>
*/
```

---

## 📸 Screenshots (Add to /assets folder)

Consider adding these screenshots to your repository and referencing them in the gallery:

| Screen | Description |
| --- | --- |
| **Onboarding** | User registration with first name, last name, email, and phone fields |
| **Home Screen** | Hero section "Little Lemon – Chicago" with Mediterranean description |
| **Menu** | Category toggles (starters/mains/desserts/drinks) with search and filtered list |
| **Detail Item** | Full-screen dish view with image, title, description, and price |
| **User Profile** | Personal information edit screen with toggle settings |

To add screenshots:
1. Add images to `LittleLemonApp/assets/` or repo root `/assets/`
2. Commit and push
3. They'll automatically appear in your GitHub Pages site if you set up an image gallery

---

## 🛠 Project Improvements Checklist

Based on code review, here are targeted enhancements you can make:

### High Priority
- [ ] **Add screenshot assets** to `/assets` folder and update README gallery
- [ ] **Add unit tests** for `ViewModel.validateUserInput()` using XCTest
- [ ] **Handle network errors** gracefully in `MenuList.getMenuData()` (show alert if API fails)
- [ ] **Add dark mode support** for all color assets (`primaryColor1`, `primaryColor2`, etc.)
- [ ] **Fix keyboard dismissal** – current implementation doesn't dismiss keyboard on tap outside text fields

### Medium Priority
- [ ] **Add search debounce** – currently triggers on every character; add a 0.5s delay for better performance
- [ ] **Improve CoreData preview** – add more sample dishes in `Persistence.oneDish()` for better preview rendering
- [ ] **Add logout animation** – smooth transition when navigating from Profile back to Onboarding
- [ ] **Add accessibility labels** to all interactive elements (images, buttons, text fields)

### Low Priority (Polish)
- [ ] **Add unit tests** for CoreData operations (`PersistenceController.clear()`, `oneDish()`)
- [ ] **Refactor Header** – currently has its own `@State var isLoggedIn`; could use `@Environment(\.managedObjectContext)`
- [ ] **Add iPad split-view support** for MainScreen and DetailItem
- [ ] **Localization** – extract hardcoded strings into `LocalizedStringKeys`

---

## 📬 Contact & Portfolio

- **GitHub**: [@ongunakaycom](https://github.com/ongunakaycom)
- **Project**: [Little-Lemon-Food-Ordering-App](https://github.com/ongunakaycom/Little-Lemon-Food-Ordering-App)
- **Portfolio Site**: Deploy this enhanced README to GitHub Pages for a professional showcase
- **Email**: info@ongunakay.com (update if needed)

---

*Built with ❤️ during the Meta iOS Developer Professional Certificate program on Coursera.*