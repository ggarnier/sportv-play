```js
class Alert extends Component {
  getStyles() {
    const status = {
      notification: "#0074D9",
      success: "#27AE60",
      error: "#E74C3C"
    }

    return {
      alert: {
        position: "relative",
        width: "100%",
        padding: "5px",
        borderRadius: "3px",
        backgroundColor: status.notification,
        color: "white",
        textAlign: "center",
        fontFamily: "'Helvetica Neue', sans-serif",
        success: {
          backgroundColor: status.success
        },
        error: {
          backgroundColor: status.error
        },

        "@media (min-width: 320px)": {
          fontSize: "15px"
        }
      },
      closeButton: {
        position: "absolute",
        right: "10px",
        color: color(status[this.props.type]).lighten(0.2).hexString(),
        ":hover": {
          color: color(status[this.props.type]).lighten(0.5).hexString(),
          cursor: "pointer"
        }
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
