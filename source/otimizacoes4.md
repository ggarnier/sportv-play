# Cachear callbacks

```js
const sum = (a, b) => a + b

const bind1 = sum.bind(this)
const bind2 = sum.bind(this)

bind1 == bind1 // false
bind1 == bind2 // false
```
