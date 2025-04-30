📘 Smart Todo List – Documentation
📌 Overview
The Smart Todo List is a responsive, interactive task management web application built with HTML, CSS, and JavaScript. It allows users to create, view, manage, and persistently store tasks with due dates using the browser’s local storage. It also features real-time date and time display, animated transitions, and responsive UI design.

🖥️ Technologies Used
HTML5 – Structure of the webpage.

CSS3 – Styling and animations for an enhanced UI/UX.

JavaScript (ES6+) – Application logic and data management.

LocalStorage API – Persistent data storage across sessions.

📋 Features
✅ Add new tasks with a title and due date/time.

📆 Display current date and time, updating every second.

📚 Store tasks in local storage to retain data on page reload.

✔️ Mark tasks as completed/undone with one click.

❌ Delete tasks with a dedicated delete button.

🖼️ Smooth fade-in and slide animations for UI transitions.

📱 Fully responsive design for all screen sizes.

🧱 File Structure
index.html
The main HTML file that contains:

Page layout and structure.

The todo form for adding tasks.

An unordered list (<ul>) for displaying tasks.

<style> (CSS)
Embedded styling that includes:

Variables for primary and secondary colors.

Responsive layouts for .container, .todo-form, .todo-list, etc.

Animations like fadeIn and slideIn.

Hover and transition effects for interactivity.

<script> (JavaScript)
Handles:

Task creation via form input.

LocalStorage integration to persist tasks.

Date/time rendering with a 1-second interval update.

Functions: addTodo(), renderTodos(), saveTodos(), loadTodos(), toggleComplete(), and deleteTodo().

⚙️ Function Breakdown
addTodo(text, dateTime)
Adds a new task object to the todos array and updates local storage.

renderTodos()
Displays all tasks from the todos array into the DOM. It adds animation and marks completed tasks visually.

toggleComplete(index)
Toggles the completion status of a task, updates local storage, and re-renders the list.

deleteTodo(index)
Removes the task at the given index and updates both the list and storage.

saveTodos(todos)
Saves the task list to localStorage under the key todoItems.

loadTodos()
Retrieves the task list from localStorage. Returns an empty array if none exist.

updateDateTime()
Updates the header with the current date and time, refreshed every second.

🧠 Local Storage Schema
json
Copy
Edit
[
  {
    "text": "Example Task",
    "dateTime": "2025-05-01T14:00",
    "completed": false,
    "createdAt": "2025-05-01T12:00:00.000Z"
  }
]
📝 How to Use
Open the webpage in any modern browser.

Type a task in the input field.

Select a due date and time.

Click “Add Task”.

Click “Complete” to mark it as done or “Delete” to remove it.

All tasks are stored locally and persist after refreshing the page.

