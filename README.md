For JavaScript;
WANJIKU HANANNY 
REG NO /00107/SS    
I started by initializing the variables by using the const taskList =document. getElementById('task-list');, Which retrieves a reference to an HTML element with the id "task-list" using the document. getElementById() method and so the variable taskList that holds the reference
And this is done to all the variables in the html for example new_task, success_message, add_task as expressed in the JavaScript document code.
 Then I added the array called (tasks) by using let tasks = []; and this is used to store all the tasks that a user adds to the to-do list.
The function loadTasks()which is responsible for loading the tasks of the todo list.
const storedTasks = localStorage.getItem('tasks'); the const storedTasks gets the stored tasks and the localStorage.getItem this gets data from the local storage where the Local storage allows you to store data persistently on the user's browser, JSON.parse() is used to convert the JSON string back into a JavaScript object and the saveTask is used to save the task in the user’s browser and this function ensures that the task stays on the page even if it is closed.
Then I used this function function renderTasks () {taskList.innerHTML = ''; // Clear the task list tasks. forEach((task) => {which ensures that each task is rendered on the user’s interface and this function helps the todo list to be flexible and scalable 
After there I used an element const checkbox = document. createElement('input'); that controls the input that the user inputs in the list
An event listener is added to the checkbox to handle changes in its state and the changes are saved to local storage by the saveTasks () 
Then I used const taskText = document.createElement('span'); to create a new html element using the document.createElement('span') method, from there I used the taskText.classList.add('task-text'); which adds a CSS class 'task-text' to the <span> element.and this allows consistent styling and so this span displays the text of the task from there I encountered the edit method were the  const editBtn =document.createElement('button'); this creates creates a new <button> element and assigns it to the variable editBtn.     editBtn.classList.add('edit-btn'); it adds a CSS style for styling purposes
editBtn.textContent = 'Edit'; which is set to edit the task.  editBtn.addEventListener('click', () => { ... }); this event listener adds the click event to the task const newText = prompt ('Edit task:', task.text); this provides the user with the box for editing the text and this is also done for the delete and the confirmation message that confirms with the user if they are sure that the task should be deleted  
After that I The code actions.appendChild(editBtn); is appending the editBtn element as a child node to the actions div. This means that the editBtn will now be a part of the actions div and will be displayed wherever the actions div is displayed. Same applies to the delete 
The code listItem.appendChild(checkbox); is appending the checkbox element as a child node to the listItem element. This means that the checkbox will now be a part of the listItem and will be displayed wherever the listItem is displayed, and this applies to the taskText and the actions which include the delete and the edit
The code if (task.completed) { listItem.classList.add('completed'); } is checking if the task object has a completed property set to true. If it does, then the listItem element will have the completed class added to it.
function addNewTask() this is responsible for adding a new task in the todo list . 
