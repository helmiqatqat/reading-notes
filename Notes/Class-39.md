# Redux - Additional Topics

## Redux Toolkit (RTK)

**What concerns are addressed by Redux Toolkit?**

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

1. "Configuring a Redux store is too complicated".
2. "I have to add a lot of packages to get Redux to do anything useful".
3. "Redux requires too much boilerplate code".

**What does configureStore() do?**

- It initializes a Redux store with some default configurations like middleware setup.

**How would I use createSlice()?**

- You'd use createSlice() to generate Redux action creators and reducers by defining a slice of the Redux store, specifying an initial state, and defining reducer functions for actions.

## MobX

**What is Mobx?**

- MobX automatically derives the state from observable sources and reactions, ensuring that everything remains consistent without the need for manual intervention.

**How does MobX make it “impossible” to produce an inconsistent state?**

- MobX automatically derives the state from observable sources and reactions, ensuring that everything remains consistent without the need for manual intervention.

**How would we build a reactive user interface?**

- Use observables in your state, and components (like those from React) would react to changes in these observables by re-rendering automatically when the state they observe changes.
