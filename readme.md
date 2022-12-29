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
```

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
