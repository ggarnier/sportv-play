```js
class Alert extends Component {
  getStyles() {
    const status = {
      success: "#27AE60",
      error: "#E74C3C"
    }
    return {
      alert: {
        success: { backgroundColor: status.success },
        error: { backgroundColor: status.error },
        "@media (min-width: 320px)": { fontSize: "15px" }
      },
      closeButton: {
        color: color(status[this.props.type]).lighten(0.2).hexString(),
      }
    }
  }

  render() {
    const styles = this.getStyles()
    return (
      <div style={[styles.alert, styles.alert[this.props.type]]}>
        { this.props.message }
        <span style={styles.closeButton}>&#x2715;</span>
      </div>
    )
  }
}
```
