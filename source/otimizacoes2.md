# Stateless components

https://hackernoon.com/react-stateless-functional-components-nine-wins-you-might-have-overlooked-997b0d933dbc

```js
const Footer = (props) => {
  return (
    <footer>
      <p>© 2017 Globo Comunicação e Participações S.A.</p>
      <a href={props.url}>Política de Privacidade</a>
    </footer>
  )
}
```
