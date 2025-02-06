# To-Do List
A todo list web app build in React.

# Project Notes
## User Stories
* read a list of tasks.
* add a task using the mouse or keyboard.
* mark any task as completed, using the mouse or keyboard.
* delete any task, using the mouse or keyboard.
* edit any task, using the mouse or keyboard.
* view a specific subset of tasks: All tasks, only the active task, or only the completed tasks.

# React Notes
* **Comments** are technically Javascript, so should be within {} braces.
* **Props** - let you pass data into React components. They can only be passed from parent components to child components. Example of passing a `subject` prop to the `App` component: `<App subject="Clarice" />` 
* Optional Chaining using the `?.` operator allows checking if a value is undefined or null before trying to operate on it, e.g. `const taskList = props.tasks.map((task) => task.name);`