# CSS in JS

```js
import disabledColor from "./constants"

class HelloWorld extends Component {
  state = {
    enabled: true
  }

  render() {
    const styles = {
      marginBottom: "5px",
      color: this.state.enabled ? "red" : disabledColor
    }

    return (
      <div style={styles}>
        Hello, world!
      </div>
    )
  }
}
```

<span class="fragment current-only" data-code-focus="11"></span>
