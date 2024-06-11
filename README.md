# Task List Application

## Overview
The Task List Application is a simple command-line program written in Java that allows users to manage a list of tasks. Users can add, remove, and list tasks through a menu-driven interface. The application keeps running until the user chooses to quit.

## Features
1. **Add Task**: Allows the user to add a new task to the list.
2. **Remove Task**: Allows the user to remove an existing task from the list by specifying the task number.
3. **List Tasks**: Displays all tasks currently in the list.
4. **Quit**: Exits the application.

## How to Run
1. Ensure you have Java installed on your system.
2. Copy the code into a file named `TaskListApp.java`.
3. Open a terminal or command prompt and navigate to the directory containing the `TaskListApp.java` file.
4. Compile the Java program using the following command:
   ```sh
   javac TaskListApp.java
   ```
5. Run the compiled Java program using the following command:
   ```sh
   java TaskListApp
   ```

## Usage Instructions
1. **Start the Program**: Run the program using the instructions above.
2. **Menu Options**: After starting the program, you will be presented with a menu with the following options:
   ```
   Task List Application
   1. Add Task
   2. Remove Task
   3. List Tasks
   4. Quit
   Select an option: 
   ```
3. **Add a Task**:
   - Select option `1` by typing `1` and pressing Enter.
   - Enter the name of the task and press Enter.
   - The task will be added to the list, and you will see a confirmation message.

4. **Remove a Task**:
   - Select option `2` by typing `2` and pressing Enter.
   - If there are tasks in the list, they will be displayed with numbers.
   - Enter the number of the task you want to remove and press Enter.
   - The task will be removed from the list, and you will see a confirmation message.
   - If there are no tasks, you will see a message indicating that there are no tasks to remove.

5. **List Tasks**:
   - Select option `3` by typing `3` and pressing Enter.
   - All tasks in the list will be displayed.
   - If there are no tasks, you will see a message indicating that there are no tasks to list.

6. **Quit the Program**:
   - Select option `4` by typing `4` and pressing Enter.
   - The program will exit.

## Code Breakdown
### Main Class: `TaskListApp`
- **main method**: Contains the main logic for displaying the menu, getting user input, and calling appropriate methods in the `TaskList` class.
- **displayMenu method**: Displays the menu options to the user.
- **getUserChoice method**: Gets the user's menu choice.
- **getTaskName method**: Prompts the user to enter a task name.
- **getUserInput method**: Prompts the user to enter an integer input.

### Helper Class: `TaskList`
- **tasks field**: An `ArrayList` that stores the list of tasks.
- **addTask method**: Adds a new task to the list.
- **removeTask method**: Removes a task from the list by its number.
- **listTasks method**: Lists all tasks in the list.
- **isEmpty method**: Checks if the task list is empty.
- **isValidTaskNumber method**: Checks if the given task number is valid.

## Example
```
Task List Application
1. Add Task
2. Remove Task
3. List Tasks
4. Quit
Select an option: 1
Enter task name: Buy groceries
Task added.

Task List Application
1. Add Task
2. Remove Task
3. List Tasks
4. Quit
Select an option: 3
1. Buy groceries

Task List Application
1. Add Task
2. Remove Task
3. List Tasks
4. Quit
Select an option: 2
1. Buy groceries
Enter the task number to remove: 1
Task removed.

Task List Application
1. Add Task
2. Remove Task
3. List Tasks
4. Quit
Select an option: 4
```

## Notes
- Ensure to handle invalid inputs properly to prevent the application from crashing.
- This application uses basic Java concepts such as loops, conditionals, ArrayList, and Scanner for user input.

Enjoy managing your tasks with this simple Java application!
