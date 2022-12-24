# The State Initialiser Pattern

When you build the component you make it possible for the user to set the `initialState` of that component.

And also make it possible for any point in time to reset the state of the component to the `initialState`

---

## How usePrevious work

```
const usePrevious = (value) => {
  const ref = useRef();
  useEffect(() => {
    ref.current = value;
  });
  return ref.current;
};
```

`useEffect` is never called until the return statement of the functional component is never reached

As soon as you call `useClapState` with initial state, the count is passed to the `usePrevious`

First time the `usePrevious` is called the return value is `undefined`

> This is **undefined** because the ref object is created without an initial value passed in i.e. useRef(nothingPassedInHere)

The second time you go ahead and click, we call `usePrevious` again. This time count is now 1.

The ref object is not re created because it was created before. `ref.current` is now 0.

Until the next invocation when it takes in 2 then it returns 1. It updates the current to 2 but never returns that

// undefined, 1, 2

---
