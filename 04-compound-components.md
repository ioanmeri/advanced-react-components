# Compound Components

Expose all the child components to the user and the `MediumClap` still.

Benefits we get out of this are

- **Customizability**

- **Understandable API**

- Avoid **Props Overload**

```
<MediumClap
  clapProps={}
  countTotalProps={}
  clapIconProps={}
/>
```

Every single prop you pass, is gonna get in `<MediumClap />` and is gonna be passed further down to the child components, and this is not necessary yet.
