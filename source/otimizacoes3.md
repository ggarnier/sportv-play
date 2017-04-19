# Cachear callbacks

```js
class VideoList extends Component {
  thumbClick() {
    metrics.register(`click video-list #{this.props.name}`)
  }

  render() {
    <VideoThumb title="video 1" onClick={this.thumbClick.bind(this)}>
    <VideoThumb title="video 2" onClick={this.thumbClick.bind(this)}>
  }
}
```
