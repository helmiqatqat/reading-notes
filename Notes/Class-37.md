# Redux - Combined Reducers

## Multiple Reducers Example

**Why create multiple reducers?**

- To make the code base readable and decrease complexity.

**How would you combine multiple reducers?**

- By importing combineReducer from redux and declare a variable that holds the combineReducer, inside the combineReducer function we pass and object contains the key as the reducer name and value of the reducer it self.

**How will you manage state as an immutable object? why?**

- By setting state rest parameter and comma the name of the action and the set the action payload to it, to always return our new state.

## Redux Docs: Using Combined Reducers

**combineReducers is a utility function to simplify the most common use case when writing ___ _____ .**

- Redux reducers

**Explain how combineReducers assembles the new state tree.**

- combineReducers is a utility provided by Redux. It takes an object whose values are different reducing functions and returns a new reducer function. When this new reducer is invoked, it calls each of the provided reducer functions with the portion of the state tree they manage and the current action, and then combines their results into a single new state tree.

**How would you define initial state in an app using combineReducers?**

- Each reducer provided to combineReducers is responsible for providing its own initial state. This means that if the state passed to the combined reducer is undefined, each child reducer is invoked with undefined for its state and should return its own initial state.

## Redux Docs: Combined Reducer Syntax

**Why will you want to split your reducing functions as your app becomes more complex?**

Splitting your reducing functions, often referred to as reducer composition, is advantageous for several reasons:

- Maintainability: Smaller, single-purpose reducers are easier to understand, maintain, and test.
- Separation of Concerns: Each reducer can focus on one specific slice of the state, ensuring that the logic is well-isolated.
- Reusability: By decoupling reducers from each other, you can potentially reuse them in different parts of your application or even in different projects.
- Scalability: As the application grows, you can continue adding reducers without bloating existing ones. This scalability is essential for large applications or teams.

**The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.**

- The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

**What is a popular convention when naming reducers?**

- A popular convention when naming reducers is to use nouns that describe the state slice they manage. For instance, if you have a reducer managing a list of users, it might be named usersReducer. If another reducer is managing the visibility filter for a list, it might be called visibilityFilterReducer. The key is to make the name descriptive enough that developers can easily infer what state slice the reducer is responsible for.
