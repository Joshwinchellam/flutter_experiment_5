# Flutter Exercise 5 – Implementation of Navigation and Routing

## Aim
To understand and implement navigation and routing in Flutter, enabling users to move between multiple screens and pass data between them using named routes.

## Description
This application has two screens: Student Details and Student Result. The user enters a student's name, registration number, and marks for three subjects. The details are stored in a `User` data model and passed to the result screen through named route arguments.

## Features
- Student name and registration number input.
- Three subject mark inputs.
- Validation for empty fields.
- Validation that marks are numeric and between 0 and 100.
- Named-route navigation from the details screen to the result screen.
- Displays subject marks, total, average, and percentage.
- Back navigation to the details screen.

## Flutter concepts used
- `MaterialApp` named routes and `initialRoute`.
- `Navigator.pushNamed()` to open the result screen.
- `Navigator.pop()` to return to the previous screen.
- `ModalRoute.of(context)!.settings.arguments` to retrieve passed data.
- A `User` model to store student information and calculate results.
- `Form`, `TextFormField`, and validators for input validation.

## Calculations
- Total = mark 1 + mark 2 + mark 3
- Average = total / 3
- Percentage = (total / 300) * 100

## Project structure
```text
flutter_ex5_student_performance/
├── lib/
│   ├── main.dart
│   ├── models/
│   │   └── user_data_model.dart
│   └── screens/
│       ├── home_screen.dart
│       └── second_screen.dart
├── pubspec.yaml
├── README.md
└── .gitignore
```

## Source status
This repository contains the Flutter source files and project configuration. The app has not been built or executed in this environment. A Flutter SDK is required to run or build it.

## Run locally (optional)
```bash
flutter pub get
flutter run
```
