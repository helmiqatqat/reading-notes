# Component Based UI

## React Quick Start

**What are the building blocks of a React app?**

- React apps are made out of components. A component is a piece of the UI (user interface) that has its own logic and appearance. A component can be as small as a button, or as large as an entire page.

**What is the difference between an HTML element and a React component?**

- HTML element's first letter is lowercase while in React component it is uppercase, React component is simply a functional component, while HTML element is a markup element.

**What is JSX and why do we use it?**

- It stands for JavaScript and XML, we use it to write both JavaScript logic and HTML elements inside on component.

**Describe the process of embedding JavaScript expressions in JSX.**

- We can escape from markup into JavaScript by using curly braces where we can write our logic.

**Does React or JSX have any special features for iteration or conditional logic?**

- In React, there is no special syntax for writing conditions. Instead, you’ll use the same techniques as you use when writing regular JavaScript code.

**How does React know to respond to a user’s inputs?**

- By triggering an event.

**What word indicates that a React component manages data with a Hook?**

- The word _use_

**How can two react components share data?**

- By moving the state to be shared into to the closest component containing all of them.

## Render and Commit

**What are the three steps of refreshing a React UI?**

- Triggering a render.
- Rendering the component.
- Committing to the DOM.

**How do you trigger updates to a component after the initial render?**

- By updating its state.

**Does React recreate DOM nodes on every rerender?**

- No. After the initial render, React DOM only rerenders the components that their state have been updated. In other terms, React only changes the DOM nodes if there’s a difference between renders. For example, here is a component that re-renders with different props passed from its parent every second.

**After React has updated the DOM, what still needs to happen before the user sees the change?**

- After rendering is done and React updated the DOM, the browser will repaint the screen. Although this process is known as “browser rendering”, we’ll refer to it as “painting” to avoid confusion throughout the docs.
