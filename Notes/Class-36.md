# Application State with Redux

## Dan Abramov Redux Tutorials

**What is the first principle of Redux?**

The first principle of Redux is that the entire state of your application is stored in a single source of truth, the state tree (or store). This ensures that managing the state becomes more predictable and makes it easier to track changes over time.

**What is a store and what do we use our reducers for within that store?**

A store in Redux holds the complete state tree of the application. The primary responsibility of the store is to allow components to read the state, dispatch actions, and register listeners. Reducers are pure functions that describe how the state should change in response to an action. When an action is dispatched to the store, the reducer takes the current state and that action, and returns a new state. In essence, reducers specify the state transformations based on the received actions.

**Name three Redux store methods given to us by createStore and describe their use.**

dispatch(action): It is used to send (or "dispatch") actions to the store. The store then updates its state based on the given action using the reducer.

getState(): This method returns the current state of the store. It's useful when you want to retrieve the current state value.

subscribe(listener): This allows you to register a callback function (listener) that will be called any time an action is dispatched, and some part of the state may potentially have changed. This is often used to let the application know when it needs to re-render or update its view in response to state changes.

**Explain to a non-technical recruiter what combineReducers() does and why it is useful.**

Alright, imagine you're organizing a big event, and you have different teams handling different tasks, like one team for catering, another for entertainment, and another for logistics. Now, instead of you managing all the details of every team, each team gives you a summary of their plan. combineReducers() in Redux is somewhat like gathering all these summaries into one master plan.

In technical terms, as applications grow, their state becomes more complex. Instead of having one huge reducer to manage this state, we break it down into smaller reducers, each managing a specific part of the state (like one for user data, another for app settings, and so on). combineReducers() takes these smaller reducers and combines them into one big reducer so the Redux store can use it. This way, our code remains organized, clean, and easier to maintain.
