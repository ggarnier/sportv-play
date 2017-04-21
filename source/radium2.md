```js
class Alert extends Component {
  getStyles() {
    return {
      alert: {
        backgroundColor: "white",
        ":hover": { cursor: "pointer" },
        "@media (min-width: 320px)": { fontSize: "15px" },

        success: { backgroundColor: "green" },
        error: { backgroundColor: "red" }
      }
    }
  }

  render() {
    const styles = this.getStyles()
    return (
      <div style={[styles.alert, styles.alert[this.props.type]]}>
        { this.props.message }
      </div>
    )
  }
}
```

<span class="fragment current-only" data-code-focus="6-7"></span>
<span class="fragment current-only" data-code-focus="18"></span>
