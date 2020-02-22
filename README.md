# remarkable-wikilink

This is a plugin for the [Remarkable][] markdown parser which adds
`[[MediaWiki-style links]]`.

## Usage

```js
const { Remarkable } = require('remarkable')
const md = new Remarkable
md.use(require('remarkable-wikilink'))

const html = md.render(`This is a [[Test]].`)
// <p>This is a <a href="Test">Test</a></p>
```

[Remarkable]: https://github.com/jonschlinkert/remarkable
