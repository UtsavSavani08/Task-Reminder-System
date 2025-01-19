# Task Management System

## Overview

The Task Management System allows you to manage tasks, where each task has a `title`, a `dueTime`, and a `priority`. The system provides functionality to add tasks, sort them by priority, filter tasks that are due within a specified time, and send reminders when tasks are due.

## Features
- **Add Tasks**: Add tasks with a title, due time, and priority.
- **Sort Tasks by Priority**: Sort tasks by their priority, with higher priority tasks appearing first.
- **Get Tasks Due within a Timeframe**: Filter and get tasks that are due within a given number of minutes.
- **Send Reminders**: Automatically sends reminders when a task is due.

## Functions

### `addTask(title, dueTime, priority)`

Adds a new task to the task list.

#### Parameters:
- `title` _(string)_: The title or description of the task.
- `dueTime` _(number)_: The number of minutes from the task's creation time when the task is due.
- `priority` _(number)_: The priority level of the task. A higher number indicates a higher priority.

#### Description:
- This function creates a new task object with the provided parameters and adds it to the `tasks` array.
- If any required field (`title`, `dueTime`, or `priority`) is missing, an error will be thrown and logged to the console.

#### Example:
```javascript
addTask("Run", 3, 1);
