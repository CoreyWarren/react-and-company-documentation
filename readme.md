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

Redux is a state management tool.  https://redux.js.org/tutorials/fundamentals/part-1-overview
It uses store, reducer, state, ui, and dispatch/actions in order to update the state of your app on a single page.

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
