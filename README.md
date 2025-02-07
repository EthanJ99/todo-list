# To-Do List
A todo list web app build in React.

## Project Notes
**User Stories**
* read a list of tasks.
* add a task using the mouse or keyboard.
* mark any task as completed, using the mouse or keyboard.
* delete any task, using the mouse or keyboard.
* edit any task, using the mouse or keyboard.
* view a specific subset of tasks: All tasks, only the active task, or only the completed tasks.

## React Notes
* **Comments** are technically Javascript, so should be within `{}` braces, e.g. `{/* Javascript comments must be nested in braces */}`.
* **Props** - let you pass data into React components. They can only be passed from parent components to child components. Example of passing a `subject` prop to the `App` component: `<App subject="Clarice" />` 
  * Props are *immutable* - a component cannot change or create it's own props.
* **Optional Chaining** using the `?.` operator allows checking if a value is undefined or null before trying to operate on it, e.g. `const taskList = props.tasks?.map((task) => task.name);`
* You should always pass a unique `key` prop to any component rendered with iteration, otherwise you might see strange behaviour/issues while rendering.
  * e.g. `<Todo id={task.id} name={task.name} completed={task.completed} key={task.id} />`
* **Callback props** can be used to pass information from a child component back to its parent. You pass a function from parent to child, which the child can then call to pass information to it's parent. e.g.
  * In Form.jsx: `function addTask(name) { alert(name); }`
  * In App.jsx: `<Form addTask={addTask} />`
* **State** can give components memory and enable communication between them using the `useState()` hook.
* **Hooks** - special category of functions which can add new functionality to a component.
* **Spread Syntax** can be used to make a copy of an array, e.g. `const arr2 = [...arr]`. You can also add new elements to existing arrays like this: `const arr2 = [...arr]`.
