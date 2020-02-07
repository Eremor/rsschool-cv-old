# Smirnov Artem
## Contact info:
* __City:__ Kazan
* __Email:__ eremid@yahoo.com
* __Skype:__ set..13
## Summary
My main goal is to change professional activities. At the moment, I work as a systems engineer and I understand that I have come to the point where I do not have enough current work intellectually, therefore, I began to actively study programming. For these purposes, I try to allocate as much time as possible and "absorb" the information with great zeal.
## Skills
* HTML5
* CSS3
* JavaScript
* BEM
* Sass
* Bootstrap
## Code examples
```
var list = document.querySelector('.todo-list');
var items = list.children;
var emptyListMessage = document.querySelector('.empty-tasks');
var newItemForm = document.querySelector('.add-form');
var newItemTitle = newItemForm.querySelector('.add-form-input');
var taskTemplate = document.querySelector('#task-template').content;
var newItemTemplate = taskTemplate.querySelector('.todo-list-item');

var toggleEmptyListMessage = function () {
  if (items.length === 0) {
    emptyListMessage.classList.remove('hidden');
  }
};

var addCheckHandler = function (item) {
  var checkbox = item.querySelector('.todo-list-input');
  checkbox.addEventListener('change', function () {
    item.remove();
    toggleEmptyListMessage();
  });
};

for (var i = 0; i < items.length; i++) {
  addCheckHandler(items[i]);
}

newItemForm.addEventListener('submit', function (evt) {
  evt.preventDefault();

  var taskText = newItemTitle.value;
  var task = newItemTemplate.cloneNode(true);
  var taskDescription = task.querySelector('span');
  taskDescription.textContent = taskText;
  addCheckHandler(task);

  list.appendChild(task);
});
```
## Experience
Examples of my work are available here: [GitHub](https://github.com/Eremor?tab=repositories)
## Education
I graduated from Almetyevsk State Oil Institute with a degree in industrial control system
Also, during my professional career, I took many courses at companies:
* Microsoft
* HP
* Kaspersky
* Veeam
* Oracle
* HTMLacademy
## English - A1
