# Context API - Behaviors

## Scaling Up with Reducer and Context

How do useReducer and useContext work together to simplify state management in a React application? (At least two paragraphs of prose)

- To combine useReducer and useContext we do the following:
  - Create the context.
    - We create context for states, and another one for dispatch function.
  - Put state and dispatch into context.
    - We wrap the parent with states context provider with value of states passed.
    - We wrap the parent with dispatch context provider with value of dispatch function passed.
  - Use context anywhere in the tree.
  