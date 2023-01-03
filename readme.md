# &#x1F4D9; Part 1 -- Summary:

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

## Base Languages/Technologies Used:

- Python
- JavaScript
- HTML
- CSS

# &#x1F4D9; Part 2 -- Breakdowns:

## How the major components work to make a web application:

- <h2>&#x1F34F; JavaScript</h2>

  <h3> Basics:</h3>
  
  - **Scope** - refers to the part of a program in which a variable is visible or accessible. There exists global scope and local scope. When a variable is defined inside a function in JS, it has local scope. When defined outside a function, it will have global scope, generally speaking.
 ```js
 function myFunction() {
 let y = 10; // y has local scope
 console.log(y); // y is accessible inside the function
 }
 ```
  
 ```js
 let x = 5; // x has global scope

 function myFunction() {
 console.log(x); // x is accessible inside the function
 }
 ```
  
  - Callbacks 
  
  - Promises
  
  - Passing Functions to other Functions 
  
  - References vs Values
  
  - == and ===, Type Coercion
    * Implicit Type Coercion:
  
    * Explicit Type Coercion
  
    * Comparison Type Coercion
  
  - Advanced Logic (Short Circuiting and More)
  
  * Order of Operations (Ands, Ors, and other Operators)
  
  * Advanced Array Methods (Math, Filter, Sort) (How Arrays are Modified)
  
  * Immutability and Modifications in JS
  
  * Asynchronous Code (Using callbacks, promises, and asyncwait)
  
  * Modules and Modularity via Small components (import, export)
  
  * ES6 new functionalities
  
  
  
  
  

- <h2>&#x1F34F; React</h2>

React is a JS (JavaScript) library used for building UIs on web apps. It allows us to build reusable UI components. These components can be combined to create more complex user interfaces. It uses a virtual Document Object Model (VDOM) to update the interface efficiently only when the underlying data changes. In other words, React only updates the parts of the interface that are necessary, avoiding re-rendering the entire UI every time changes are made.

When combined with other libaries, frameworks, and techniques such as Express, Redux, AJAX, and Django, which are all listed below as components for this project archetype, complete web applications can be created. 
```js
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
  
**React Apps consist of:**

- Components: Components are the building blocks of a React app. They are reusable pieces of UI that can be combined to create complex user interfaces. Components can be classified as either functional or class-based. Functional components are simple functions that take props as an argument and return a JSX element, while class-based components are classes that extend the React.Component base class and define a render method.

- Props: Props (short for "properties") are inputs to a component that are passed in from the parent component. They are used to customize the behavior and appearance of a component and can be accessed inside the component using the props object.

- State: State is a data store for a component that is managed by the component itself. It is used to store data that is specific to the component and can change over time. State is initialized when the component is created and can be updated using the setState method.

- Routing: Routing is the process of defining the paths and components that should be displayed for different URL patterns in a single-page application. It is often handled using a routing library like react-router, which provides a set of components and functions for defining and navigating between routes.

- API integration: Many React apps need to interact with APIs to retrieve data or perform actions. This can be done using a library like axios or the fetch API to make HTTP requests and handle the responses.

- Testing: Testing is an important part of the development process for any app. React apps can be tested using a variety of tools, such as Jest for unit testing and Enzyme for integration testing.

There are many other aspects of building a production-ready React app, such as building and deploying the app, optimizing performance, and handling errors and edge cases.




- <h2>&#x1F34F; Redux</h2>

Redux is a state management tool for JavaScript applications. It helps you design applications that behave consistently and are easy to test by keeping the application state in a single, immutable store.

Here is a fellow dev's views on Redux: https://qr.ae/prvjpl

What you'll hear from https://www.youtube.com/watch?v=CVpUuw9XSjY is:

- **Store** is a globalized state. It's all the data for your entire website that you will pull from anywhere and anytime.

- **Actions** are what we want to do to our data in the store. (i.e.: I want to increment a number by 1. So our action would be "Increment."

- **Reducers** are descriptions of what we want our actions to do from the current state to the next (desired) state.

- **Dispatching** means EXECUTING your actions!

### For Redux specifically, we can break these steps into more detail:

- Initial setup:
  * A Redux store is created using a root reducer function.
  * The store calls the root reducer once, and saves the return value as its initial state
  * When the UI is first rendered, UI components access the current state of the Redux store, and use that data to decide what to render. They also subscribe to any -- future store updates so they can know if the state has changed.
- Updates:
  * Something happens in the app, such as a user clicking a button
  * The app code dispatches an action to the Redux store, like dispatch({type: 'counter/incremented'})
  * The store runs the reducer function again with the previous state and the current action, and saves the return value as the new state
  * The store notifies all parts of the UI that are subscribed that the store has been updated
  * Each UI component that needs data from the store checks to see if the parts of the state they need have changed.
  * Each component that sees its data has changed forces a re-render with the new data, so it can update what's shown on the screen

- <h2>&#x1F34F; Express</h2>
```
```
- <h2>&#x1F34F; Django</h2>
```
```
- <h2>&#x1F34F; AJAX</h2>
```
```
- <h2>&#x1F34F; DigitalOcean</h2>
```
```
