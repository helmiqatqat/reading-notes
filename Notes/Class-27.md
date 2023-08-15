# React useState Hook

## Thinking in React

**Summarize the five steps of thinking in react.**

**Step 1**: Break the UI into a component hierarchy.

- Simply use single responsibility principle, dividing the UI into components make it easier for the developer to know which components goes inside which components, furthermore increase the code readability and decrease time required for maintainance, as well as scalability where it is easy to add new features.

**Step 2**: Build a static version in React.

- Build the static version where it requires no thinking and more typing, then build the interactive part where it requires thinking and less typing.

**Step 3**: Find the minimal but complete representation of UI state.

- Use the DRY method (Don't Repeat Yourself), basically identifying your app’s minimal state data.

**Step 4**: Identify where your state should live.

- It is important to determine weither the state should be used by many components where we need to find their common parent component and declare state in and pass it to the children, or used by an indivual component where we just declare the state inside that component.

**Step 5**: Add inverse data flow.

- Users inputs should get their values from states, where when ever the user changes the input it calls a function to set the state's value into the current input value, in other words user inputs should be controlled by state.

## State: A Component’s Memory

**What is one reason a local variable isn’t sufficient for managing a React component?**

- Local variables don’t persist between renders. When React renders this component a second time, it renders it from scratch—it doesn’t consider any changes to the local variables.

- Changes to local variables won’t trigger renders. React doesn’t realize it needs to render the component again with the new data.

**What is the argument to the useState hook, and what are the two parts of its return array?**

- State variable and setter function.

**How can Component A access state from Component B?**

- If A is a sibling to B, you can't unless you move the state to the closes parent component and pass the state and setter function as props.

- If A is a child of B, we can pass the state and the setter function from B to A.
