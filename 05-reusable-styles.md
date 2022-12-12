# Reusable styles

While it's not an advanced React patter itself, it's important to offer flexibility over the styles of reusable components.

**Strategy**

```
<div>Hello</div>
```

2 ways to do this in React:

1. className

```
<div className="red">Hello</div>
```

2. Inline style

```
<div style={{color: 'red'}}>Hello</div>
```

Pass className or inline style in `MediumClap`

```
<MediumClap style className="">Hello</MediumClap>
```
