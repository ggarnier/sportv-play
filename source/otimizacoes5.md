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
    <VideoThumb title="video 1" onClick={this.thumbClickCallback}>
    <VideoThumb title="video 2" onClick={this.thumbClickCallback}>
  }
}
```

<span class="fragment current-only" data-code-focus="3"></span>
<span class="fragment current-only" data-code-focus="11-12"></span>
