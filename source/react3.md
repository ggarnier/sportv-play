```js
// Modelo imperativo, c/ jQuery
$("button").prop("disabled", true)

$("textarea").on("input", function() {
  if ($(this).val().length > 0) {
    $("button").prop("disabled", false)
  } else {
    $("button").prop("disabled", true)
  }
})
```

```js
// Modelo declarativo, c/ React
class TweetBox extends Component {
  state = { text: "" }

  handleChange(event) {
    this.setState({ text: event.target.value })
  }

  render() {
    return (
      <div>
        <textarea onChange={this.handleChange}></textarea>
        <button disabled={this.state.text.length === 0}>Tweet</button>
      </div>
    )
  }
}
```
