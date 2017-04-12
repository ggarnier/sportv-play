```js
import { createStore } from 'redux'

// Create reducer
counter(state = 0, action) => {
  switch (action.type) {
  case 'INCREMENT':
    return state + 1
  case 'DECREMENT':
    return state - 1
  default:
    return state
  }
}

// Create store
let store = createStore(counter)

// React to store changes
store.subscribe(() =>
  console.log(store.getState())
)

// Dispatch actions
store.dispatch({ type: 'INCREMENT' }) // 1
store.dispatch({ type: 'INCREMENT' }) // 2
store.dispatch({ type: 'DECREMENT' }) // 1
```
