# Summary:

## Major components of this project:

- React
- Redux
- Express
- Django
- AJAX
- DigitalOcean

## Minor Components of this project:

- nginx
- bootstrap

## Languages/Technologies Used:

- Python
- JavaScript
- HTML
- CSS

# Breakdowns:

## How the major components work to make a web application:

- React

React is a JS (JavaScript) library used for building UIs on web apps. It allows us to build reusable UI components. These components can be combined to create more complex user interfaces. It uses a virtual Document Object Model (VDOM) to update the interface efficiently only when the underlying data changes. In other words, React only updates the parts of the interface that are necessary, avoiding re-rendering the entire UI every time changes are made.

When combined with other libaries, frameworks, and techniques such as Express, Redux, AJAX, and Django, which are all listed below as components for this project archetype, complete web applications can be created. 
```
import React from 'react';

const projects = [
  {
    name: 'Project A',
    description: 'A description of Project A',
    url: 'http://example.com/project-a'
  },
  {
    name: 'Project B',
    description: 'A description of Project B',
    url: 'http://example.com/project-b'
  },
  {
    name: 'Project C',
    description: 'A description of Project C',
    url: 'http://example.com/project-c'
  }
];

function App() {
  return (
    <div>
      <h1>My Portfolio</h1>
      {projects.map(project => (
        <div key={project.name}>
          <h2>{project.name}</h2>
          <p>{project.description}</p>
          <a href={project.url}>View project</a>
        </div>
      ))}
    </div>
  );
}

export default App;
```
- Redux

Redux is a state management tool for JavaScript applications. It helps you design applications that behave consistently and are easy to test by keeping the application state in a single, immutable store.

```js
import { createStore } from 'redux';

// Reducer function
function counter(state = 0, action) {
  switch (action.type) {
    case 'INCREMENT':
      return state + 1;
    case 'DECREMENT':
      return state - 1;
    default:
      return state;
  }
}

// Create a Redux store
const store = createStore(counter);

// Subscribe to the store to receive updates
store.subscribe(() => console.log(store.getState()));

// Dispatch actions to update the state
store.dispatch({ type: 'INCREMENT' }); // -> 1
store.dispatch({ type: 'INCREMENT' }); // -> 2
store.dispatch({ type: 'DECREMENT' }); // -> 1
```



The major parts of Redux are:

Store: The store is the central data store for the application. It holds the current state of the application, and is the only place where the state can be updated. The store is created using the createStore function and a reducer function, which defines how the state is updated in response to actions.

Actions (Dispatch): Actions are payloads of information that are sent to the store to update the state. They are plain JavaScript objects that must have a type property to identify the type of action being performed. Actions can also include other properties that contain additional data needed to update the state.

Reducers: Reducers are pure functions that take the current state and an action as arguments and return a new state. They define how the state is updated in response to actions. Reducers must be pure functions, meaning they should not have any side effects and should always return the same output for a given input.

Middleware: Middleware is optional code that can be added to the store to extend its functionality. It allows you to perform tasks such as logging actions, handling asynchronous actions, or dispatching additional actions.

Selectors: Selectors are functions that allow you to retrieve specific pieces of data from the store. They are typically used to extract data from the store state and transform it into a form that is more suitable for presentation or manipulation.


- Express
```
```
- Django
```
```
- AJAX
```
```
- DigitalOcean
```
```
