# Cachear callbacks

```js
class Home extends Component {
  constructor() {
    this.thumbClickCallback = this.thumbClick.bind(this)
  }

  thumbClick() {
    metrics.register(`click video-list #{this.props.name}`)
  }

  render() {
    <VideoThumb onClick={this.thumbClickCallback}>
  }
}
```
