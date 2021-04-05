# afinn-111

[![Build][build-badge]][build]
[![Coverage][coverage-badge]][coverage]
[![Downloads][downloads-badge]][downloads]
[![Size][size-badge]][size]

Easy access to [afinn-111][afinn111].

## Install

[npm][]:

```sh
npm install afinn-111
```

## Use

```js
var afinn = require('afinn-111')

afinn.positive //=> 2
afinn['self-deluded'] //=> -2
```

## API

### `afinn111`

`afinn-111` returns entries to valence ratings (`Object.<string, number>`).

> Note!
> Be careful when accessing unknown properties on the `afinn-111` object, words
> such as “constructor” or “toString” might occur.
> It’s recommended to use a `hasOwnProperty` check beforehand.

## Musings

Note the AFINN entries are:

*   All lower case
*   Can contain numbers (only case: `n00b`)
*   Can contain spaces (cases: `can't stand`, `cashing in`,
    `cool stuff`, `does not work`, `dont like`, `fed up`, `green wash`,
    `green washing`, `messing up`, `no fun`, `not good`, `not working`,
    `right direction`, `screwed up`, `some kind`)
*   Can contain apostrophes (only case: `can't stand`)
*   Can contain diaeresis (only case: `naïve`)
*   Can contain dashes (cases: `cover-up`, `made-up`,
    `once-in-a-lifetime`, `self-confident`, `self-deluded`,
    `short-sighted`, `short-sightedness`, `son-of-a-bitch`)

## Related

*   [`afinn-96`](https://github.com/words/afinn-96)
    — AFINN list from 2009, containing 1468 entries
*   [`afinn-165`](https://github.com/words/afinn-165)
    — AFINN list from 2015, containing 3382 entries
*   [`emoji-emotion`](https://github.com/words/emoji-emotion)
    — Like AFINN, but for emoji
*   [`polarity`](https://github.com/words/polarity)
    — Detect the polarity of text, based on `afinn-165` and `emoji-emotion`

## License

[MIT][license] © [Titus Wormer][author]

<!-- Definitions -->

[build-badge]: https://github.com/words/afinn-111/workflows/main/badge.svg

[build]: https://github.com/words/afinn-111/actions

[coverage-badge]: https://img.shields.io/codecov/c/github/words/afinn-111.svg

[coverage]: https://codecov.io/github/words/afinn-111

[downloads-badge]: https://img.shields.io/npm/dm/afinn-111.svg

[downloads]: https://www.npmjs.com/package/afinn-111

[size-badge]: https://img.shields.io/bundlephobia/minzip/afinn-111.svg

[size]: https://bundlephobia.com/result?p=afinn-111

[npm]: https://docs.npmjs.com/cli/install

[license]: license

[author]: https://wooorm.com

[afinn111]: https://www2.imm.dtu.dk/pubdb/views/publication_details.php?id=6010
