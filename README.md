# React/TypeScript Redux Todo App

- [DEMO LINK](https://denlysiak.github.io/todo-react-TS-redux-app/)

The application is build using React with Typesciprt. As state manager Redux was used. To create resposive and user friendly layout,  'SCSS' modules were used and 'FontAwesome' to provide some fonts. To provide smooth loading and todo adding animation 'TransitionGroup' library is used.

Folder structure includes: 
  - 'api' folder with methods to change, add, or delete 'todos' throught making server requests by using URL address;
  - 'app' folder with customs hooks, redux 'store' file and 'features' folder with all redux slices;
  - 'components' folder with all componets sorted separate in own folder;
  - 'styles' folder consisting of custom 'scss' files needed to change UI;
  - 'types' folder with files, keeping all neccessary types in one place;
  - 'utils' folder with function wich are reused through the app;

Each component folder includes: 
  - 'Component.tsx' file with layout and important variables;
  - 'utilsComponent.ts' file with logic of the component;

Main app loading happens in 'App' component, wich passes list of filtered todos, regarding of what status is active, to 'Main' component where list renders. To imitate loading with temporary todo, separate component is shoqn until positive status of request is returned.

In 'Header' component there is 'form' to add new todo and 'toggle All' button to change the status of all todos.
In 'Footer' component there are 'status' links, indicator of uncompleted todos and 'clear All completed todos' button;
In 'TodoItem' componet there is a form wich enables editing of texts of exsisting todo, toggle button to change the status of todo, and delete button to remove todo; 
'ActiveForm' component is used to update the content of todo, an empty content will be delited, canceling of editing can be done by pressing 'ESC' button, form submition happens by click outside of form or enter button.
'Errors' component show error with corresponding message to the error, after error fires, the message will disappear after 3s.



 
