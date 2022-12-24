# The Props Getters Pattern

It's not possible for the user to change any values of a props collection

What if we make the props collection more valuable. This is what props getters do.

Props collection is an object, a prop getter is a function.

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
