# Redux - Asynchronous Actions

## async actions

**Why use Redux middleware?**

- By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

**Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.**

- So because HTTP request require time to fetch, the client action get delayed by a thunk action until the response is completed and recievd.

**How are we accommodating async in our Redux app?**

- Using thunk middleware

## thunk middleware

**Why would you need redux-thunk middleware?**

- In order to handle the HTTP requests asynchronous behaviour.

**Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.**

- Function.

**Describe how any return value from the inner thunk function will be made available.**

- Any return value from the inner function will be available as the return value of dispatch itself.
