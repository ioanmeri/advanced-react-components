# Controls props

What if user wanted to have control over the state object.

The idea comes from controlled components.

**Controlled input**

```
<input
  value={this.state.val}
  onChange={handleClap}
/>
```

Make sure that the user can pass a callback, and also pass value which represents the state values for the `MediumClap`

```
<MediumClap values={} onClap={} />
```

- state values
- state updater

---
