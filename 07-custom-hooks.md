# Custom Hooks

```
<MediumClap />
```

=> Logic + UI element(s)

What if we could break the logic into smaller modules that could be reusable e.g. smaller custom hooks

Technically, breaking complicated logic into smaller modules, helps for readability. But, it is possible that you could help with reusability as well.

Because some user of a component, might actually need one of your hooks.

---

## Example of Usage

Although we had multiple components exported

- MediumClap
- Icon
- useClapAnimation

the user only used the **useClapAnimation** we build out.

```
const Usage = () => {
  const animationTimeline = useClapAnimation({
    duration: 300,
    bounceEl: '#stream',
    fadeEl: '#cupHandle',
    burstEl: '#coffee'
  })

  const handleClick = () => {
    animationTimeline.replay()
  }

  return (
    <section className={userStyles.cupContainer}>
      <div className={userStyles.cupStream}>
        <Stream />
      </div>
      <div id='coffee' style={{ fontSize: '0.5rem' }}>
        coffee
      </div>
      <div className={userStyles.cupBody}>
        <CupHandle />
        <CupBowl />
      </div>
      <div>
        <CupBase />
      </div>
      <footer>
        <button onClick={handleClick}>Animate</button>
      </footer>
    </section>
  )
}
```
