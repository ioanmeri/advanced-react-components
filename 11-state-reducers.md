# The state reducer pattern

Split into two words. Reducer is a special function

```
(state, action) => {
  return newState
}
```

You can allow your user of your component or hook, to pass in a reducer and give them the control to update your internal state from the outside.

Similar to:

```
<MediumClap
  values={state.values}
  onChange={handleChange}
/>
```

inversion of control

but different:

```
<MediumClap
  reducer={reducer}
/>
```

---
