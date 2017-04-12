```js
import {observable, autorun} from 'mobx'

const counter = observable(0)

autorun(() => console.log(counter.get()))

counter.set(counter.get() + 1) // 1
counter.set(counter.get() + 1) // 2
counter.set(counter.get() - 1) // 1
```
