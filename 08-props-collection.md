## Props collection

What if we have a different export strategy

Export:

- custom hooks
- UI components

all of them, or some of them is totally up to you if you use them.

---

**Collection pattern**

Provide a collection that holds reused values so the user doesn't have to do this.

From:

```
<Train seat strap foo />
<Train seat strap foo />
<Train seat strap foo />
```

To:

```
<Train collection />
<Train collection />
<Train collection />
```

Collection is an object of property values for which we know the user is gonna need. Or we that of the usage of our component, this collection is going to be important for the user.

---
