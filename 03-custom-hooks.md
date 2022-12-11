## Custom hooks

Let you extract component logic into reusable functions.

Custom hook are not necessary an advanced pattern, more of a convention.

**Rules**

- the name has to start with _use_
- you can use any of the default hook
- rules of custom hooks
  - only call hooks at the top level
  - only call hooks from react functions

Notes:

- **useEffect** will not be called until the render function has been called. In functional components the render function is pretty much the return statement.
