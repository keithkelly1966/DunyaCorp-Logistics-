# To-Do List Application

A modern, feature-rich to-do list application built with HTML, CSS, and vanilla JavaScript. All data is stored locally using browser's localStorage API.

## Features

✅ **Add Tasks** - Quickly add new tasks with the input field or press Enter
✅ **Mark as Complete** - Check off completed tasks
✅ **Delete Tasks** - Remove individual tasks
✅ **Filter Tasks** - View all, active, or completed tasks
✅ **Task Statistics** - See total, active, and completed task counts
✅ **Local Storage** - All tasks are saved automatically and persist between sessions
✅ **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
✅ **Beautiful UI** - Modern gradient design with smooth animations
✅ **XSS Protection** - HTML escaping for user input

## How to Use

1. **Open the Application**
   - Simply open `index.html` in your web browser

2. **Add a Task**
   - Type your task in the input field
   - Click "Add Task" or press Enter

3. **Manage Tasks**
   - Click the checkbox to mark a task as complete
   - Click "Delete" to remove a task

4. **Filter Tasks**
   - Click "All" to see all tasks
   - Click "Active" to see incomplete tasks
   - Click "Completed" to see finished tasks

5. **Bulk Actions**
   - "Clear Completed" - Remove all completed tasks at once
   - "Delete All" - Remove all tasks (with confirmation)

## Local Storage

Your tasks are automatically saved to your browser's local storage. This means:
- Tasks persist when you close and reopen the browser
- Each browser/device stores tasks separately
- Clearing browser data will delete your tasks
- No server or internet connection needed

## Browser Support

- Chrome/Chromium (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Any modern browser with LocalStorage support

## File Structure

```
├── index.html      # HTML structure
├── styles.css      # Styling and animations
├── script.js       # Application logic
└── README.md       # Documentation
```

## Technical Details

### JavaScript Classes
- `TodoApp` - Main application class managing all todo operations

### Key Methods
- `addTodo()` - Add a new task
- `toggleTodo(id)` - Mark task as complete/incomplete
- `deleteTodo(id)` - Remove a task
- `clearCompleted()` - Remove all completed tasks
- `deleteAll()` - Remove all tasks
- `setFilter(filter)` - Apply filter (all/active/completed)
- `saveToStorage()` - Save tasks to localStorage
- `loadFromStorage()` - Load tasks from localStorage

### Data Structure
```javascript
{
    id: timestamp,
    text: "Task description",
    completed: boolean,
    createdAt: "date string"
}
```

## Future Enhancements

- 📅 Due dates for tasks
- 🏷️ Task categories/tags
- 🔄 Task priority levels
- 📱 Progressive Web App (PWA) support
- ☁️ Cloud synchronization
- 🌙 Dark mode theme
- 📊 Task analytics

## License

Open source - feel free to use and modify!
