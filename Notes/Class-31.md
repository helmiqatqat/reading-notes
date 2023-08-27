# Context API

## Choosing the State Structure

**Summarize the five principles for structuring state.**

- If two state variables always update together, consider merging them into one.
- Choose your state variables carefully to avoid creating “impossible” states.
- Structure your state in a way that reduces the chances that you’ll make a mistake updating it.
- Avoid redundant and duplicate state so that you don’t need to keep it in sync.
- Don’t put props into state unless you specifically want to prevent updates.
- For UI patterns like selection, keep ID or index in state instead of the object itself.
- If updating deeply nested state is complicated, try flattening it.

## Passing State Deeply with Context

**What problem do Contexts aim to solve?**

- Get rid of props drilling, instead giving the props to the elements that do need that prop.
- Resolves state issue in deeply nested components.

**What is one technique to try before useContext?**

- Extracting components and pass JSX as children to them.

**What hook complements useContext for complex applications?**

- useReducer.
