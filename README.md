# To-Do List Flutter Widget

A simple Flutter mobile app that lets users manage their daily tasks. 
Users can add tasks, mark them as complete, and delete them from the list.

---

## How to Run

1. Clone this repository
2. Open the project folder in VS Code
3. Run the following commands in the terminal:

```bash
flutter pub get
flutter run
```

4. Choose your preferred device (Chrome, emulator, etc.)

---

## Widget Overview

This app is built around a single StatefulWidget called `TodoListPage`.
It demonstrates how Flutter handles dynamic UI updates through state management.

---

## Three Key Attributes

### 1. StatefulWidget and setState()
`TodoListPage` extends `StatefulWidget` because the task list changes 
during runtime, tasks are added, checked, and deleted. Every time one 
of these actions happens, it is wrapped inside `setState()`, which tells 
Flutter to rebuild the UI and reflect the latest data on screen.

### 2. TextEditingController
A `TextEditingController` is attached to the `TextField` where the user 
types a new task. It allows the app to read the typed text when the Add 
button is pressed, and then clear the field immediately after the task 
is added — keeping the input ready for the next entry.

### 3. ListView.builder
Instead of hardcoding each task as a fixed widget, `ListView.builder` 
dynamically generates a `ListTile` for every item currently in the 
`_tasks` list. It uses `itemCount: _tasks.length` to know how many 
items to build, meaning the UI automatically scales whether there are 
2 tasks or 200 — without changing any code.

---

## Screenshot

<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/36a614e7-a0ca-4c42-836c-256a32fcff66" />

The screenshot above shows the app running on a Pixel 7 emulator. 
Three tasks are listed, two pending and one marked as completed, 
shown with a strikethrough. The input field and Add button at the 
top are ready for a new entry.

---

## Author

Laura KARANGWA KWIZERA






