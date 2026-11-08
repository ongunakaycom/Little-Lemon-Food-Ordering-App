# 🍋 Little Lemon – iOS Food Ordering App

![Meta](https://img.shields.io/badge/Meta-iOS%20Developer%20Certificate-1a73e8?logo=meta&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-5.7-orange?logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-5.7-blue?logo=ios&logoColor=white)
![Xcode](https://img.shields.io/badge/Xcode-14+-red?logo=xcode&logoColor=white)
![CoreData](https://img.shields.io/badge/CoreData-persistent-green?logo=database&logoColor=white)
![Combine](https://img.shields.io/badge/Combine-reactive-purple?logo=swift&logoColor=white)
![MVVM](https://img.shields.io/badge/MVVM-architecture-success?logo=react&logoColor=white)
![Coursera](https://img.shields.io/badge/Coursera-Professional%20Certificate-blue?logo=coursera&logoColor=white)

# 🍋 Little Lemon – iOS Food Ordering App

**Little Lemon** is an elegant SwiftUI iOS application for a fictional Mediterranean restaurant, built as the capstone project for the **Meta iOS Developer Professional Certificate** on Coursera. The app demonstrates modern iOS development practices including **SwiftUI**, **CoreData** for persistent storage, **MVVM** architecture, and **Combine** for reactive state management.

This project is part of the **Meta iOS Developer Professional Certificate** program – a 12-course series designed to launch careers as iOS developers. No degree or prior experience is required.

---

## 🎯 For Individuals

Launch your career as an iOS developer with job-ready skills. This program teaches you how to create applications for iOS systems, manage mobile app lifecycles, and build a portfolio projects that show your ability to publish, deploy, and maintain iOS apps as well as cross-platform apps using React Native.

**Skills you'll gain:**
- Unix Commands, Restful API, User Centered Design, User Experience Design
- Data Structures, Mobile Development, User Interface (UI)
- User Interface and User Experience (UI/UX) Design
- Figma (Design Software), GitHub, Swift Programming
- Javascript, Apple iOS, Jest (JavaScript Testing Framework)
- React Native, Apple Xcode, Core Data, Git (Version Control System)

**Shareable certificate** – Add to your LinkedIn profile, resume, or CV.

**Median salary and job opening data** are sourced from Lightcast™ Job Postings Report.

**Content Creator, Machine Learning Engineer and Salesforce Development Representative** (1/1/2024 - 12/12/2024)

**All other job roles** (11/1/2025 - 11/12/2026)

**4.6 avg rating** from 8,831 reviews across 12 courses

- 76.06% – 5 stars
- 15.96% – 4 stars
- 4.55% – 3 stars
- 1.64% – 2 stars
- 1.77% – 1 star

---

## 💼 For Businesses

Build your team's iOS development capabilities with this comprehensive 12-course program. Employees gain hands-on experience creating iOS applications, working with web technologies, managing data on iOS applications, and building cross-platform applications using React Native.

**Enterprises can:**
- Upskill teams with in-demand iOS development skills
- Build a portfolio of projects showcasing ability to publish, deploy and maintain iOS apps
- Prepare technical interviewees for iOS developer roles
- Access a shareable certificate for employee LinkedIn profiles

**Trusted by enterprises:** Petrobras, TATA, Danone, Capgemini, P&G and L'Oreal have enrolled teams in this program.

**Coursera for Business** – Professional Certificate – 12 course series

---

## 🏫 For Universities

Integrate this program into your computer science or mobile development curriculum. The Meta iOS Developer Professional Certificate provides:

- **Structured learning path** – 12 courses over 8 months at 7 hours per week
- **Hands-on activities** – Create protocols in Swift, build UIs in SwiftUI, develop native iOS mobile applications
- **Capstone project** – Complete a capstone project in the final course that can be added to portfolios and showcased during job interviews
- **University credit eligibility** – This Professional Certificate has ACE® recommendation and is eligible for college credit at participating U.S. colleges and universities

**Courses include:**
1. Introduction to iOS Mobile Application Development (12 hours)
2. Version Control (16 hours)
3. Programming Fundamentals in Swift (26 hours)
4. Principles of UX/UI Design (21 hours)
5. Create the User Interface with SwiftUI (21 hours)
6. Advanced Programming in Swift (19 hours)
7. Working with Data in iOS (19 hours)
8. Mobile Development and JavaScript (45 hours)
9. React Basics (30 hours)
10. React Native (38 hours)
11. iOS App Capstone (16 hours)
12. Coding Interview Preparation (11 hours)

**Learn more about Coursera for Campus**

---

## 📚 What You'll Learn

| Course | Hours | Key Skills |
|--------|-------|------------|
| **Course 1**: Introduction to iOS Mobile Application Development | 12 hours | iOS programming concepts, UI creation basics |
| **Course 2**: Version Control | 16 hours | Git, GitHub, version control best practices |
| **Course 3**: Programming Fundamentals in Swift | 26 hours | Swift programming, data structures |
| **Course 4**: Principles of UX/UI Design | 21 hours | User centered design, UX/UI principles |
| **Course 5**: Create the User Interface with SwiftUI | 21 hours | SwiftUI, adaptive layouts, UI best practices |
| **Course 6**: Advanced Programming in Swift | 19 hours | Advanced Swift, memory management |
| **Course 7**: Working with Data in iOS | 19 hours | Core Data, web technologies, data management |
| **Course 8**: Mobile Development and JavaScript | 45 hours | JavaScript, cross-platform foundations |
| **Course 9**: React Basics | 30 hours | React, component-based UI |
| **Course 10**: React Native | 38 hours | Cross-platform iOS/Android development |
| **Course 11**: iOS App Capstone | 16 hours | Complete iOS app, portfolio project |
| **Course 12**: Coding Interview Preparation | 11 hours | Technical interview preparation |

---

## 📁 Project Structure

This repository contains the **Little Lemon iOS Food Ordering App** capstone project built during the Meta iOS Developer Professional Certificate. The project demonstrates:

- **SwiftUI** UI design and adaptive layouts
- **CoreData** persistence and local storage
- **MVVM** architectural pattern separation
- **JSON networking** and data decoding from API
- **Unit testing** with XCTest
- **iOS app lifecycle** management

### Repository Structure

```
LittleLemonApp/
├── LittleLemonApp/                    # Xcode project folder
│   ├── Assets.xcassets/              # App icons, images
│   ├── CoreData/                      # Persistence and data models
│   ├── Models/                       # MenuItem and MenuList
│   ├── ViewModels/                   # Business logic and CoreData operations
│   ├── Views/                      # SwiftUI screens and components
│   │   ├── Onboarding.swift         # User registration flow
│   │   ├── Home.swift               # Entry point → MainScreen
│   │   ├── MainScreen.swift         # Header + Menu container
│   │   ├── Menu.swift               # Search, filters, category toggles, dish list
│   │   ├── Hero.swift               # Restaurant hero section
│   │   ├── Header.swift             # Top bar with profile avatar
│   │   ├── DetailItem.swift         # Single dish detail view
│   │   └── FoodItem.swift           # List row dish component
│   └── LittleLemonApp.swift        # App entry point
│   └── LittleLemonApp.xcodeproj/     # Xcode project file
├── .github/                         # GitHub workflows
│   ├── workflows/
│   │   ├── terraform-ci.yml         # CI/CD pipeline (from GCP project)
│   │   └── pages.yml                # GitHub Pages deployment
│   └── dependabot.yml               # Weekly updates
├── docs/                            # Static site for GitHub Pages
│   ├── index.html                   # Portfolio showcase site
│   ├── styles.css                   # Styling (from GCP project)
│   ├── script.js                    # Interactive elements
│   └── assets/                      # Preview images
├── terraform/                       # Infrastructure as code (from GCP project)
│   ├── main.tf                      # Provider, APIs, IAM, bucket, cluster
│   ├── variables.tf                 # Input variables and validation
│   ├── outputs.tf                   # Cluster ID, bucket, submit command
│   └── terraform.tfvars.example     # Example variable values
├── scripts/                         # Utility scripts
│   ├── submit_spark_pi.sh           # Submit SparkPi job via gcloud
│   └── check_plan_destroys.py       # Summarises destructive plan changes
├── .pre-commit-config.yaml         # Pre-commit hooks configuration
├── .tflint.hcl                     # Shared TFLint configuration
├── LICENSE                         # MIT License
└── README.md                        # This file
```

---

## 🛠 Technologies

| Layer | Technology |
|-------|------------|
| **Language** | Swift 5.7+ |
| **UI Framework** | SwiftUI |
| **Architecture** | MVVM (Model-View-ViewModel) |
| **Persistence** | CoreData |
| **Networking** | URLSession + Combine |
| **IDE** | Xcode 14+ |
| **Platform** | iOS (iPhone & iPad) |
| **Assessment** | 12-course Professional Certificate from Meta |

---

## 📦 Local Setup

### Requirements

- **Xcode 14+** (or newer)
- **macOS Monterey** (12+) or newer
- **Swift 5.7+**
- iOS Simulator or real device

### Run the App

```bash
# Open project in Xcode
open LittleLemonApp.xcodeproj
```

1. Select an iOS simulator or connect a physical device.
2. Press **Cmd+R** or click the "Play" button in Xcode to build and run.
3. The app launches on the **Onboarding Screen** – enter user details and tap **Register** to proceed to Home.

---

## 📄 License

This project is licensed under the **MIT License** – see the [`LICENSE`](./LICENSE) file for details.

---

## 📬 Contact & Portfolio

- **GitHub**: [@ongunakaycom](https://github.com/ongunakaycom)
- **Capstone Project**: [Little-Lemon-Food-Ordering-App](https://github.com/ongunakaycom/Little-Lemon-Food-Ordering-App)
- **Part of**: Meta iOS Developer Professional Certificate on Coursera
- **Email**: info@ongunakay.com (update if needed)

---

*Built with ❤️ during the Meta iOS Developer Professional Certificate program on Coursera. This project demonstrates skills required for entry-level iOS developer careers and can be added to portfolios for job interviews.*