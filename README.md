# To-Do app

This is a simple to-do list app created with javascript

# Live link

https://aliyo254.github.io/TodoApp/html/index.html

## Code Description

Used :
Javascript
Html 5
Css3
Bootstrap 5
Vim Editor

Copy code to the files

```bash
vim index.html
```
```bash
vim about.html
```
```bash
vim style.css
```
```bash
vim main.js
```

## Code snippet

```javascript

let addToDoButton = document.getElementById('addToDo');
let toDoContainer = document.getElementById('toDoContainer');
let inputField = document.getElementById('inputField');

addToDoButton.addEventListener('click', function(){
    var paragraph = document.createElement('p');
    paragraph.classList.add('paragraph-styling');
    paragraph.innerText = inputField.value;
    toDoContainer.appendChild(paragraph);
    inputField.value = "";
    paragraph.addEventListener('click', function(){
        paragraph.style.textDecoration = "line-through";
    })
    paragraph.addEventListener('dblclick', function(){
        toDoContainer.removeChild(paragraph);
    })
})
```

## Contributing
Pull requests are welcome.

Thank you

## License
[MIT](https://choosealicense.com/licenses/mit/)
