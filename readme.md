# romanize-korean

Node.js ES Module for romanizing Korean hangul (한글) text.

## installation

```sh
yarn add romanize-korean
```

## usage

```javascript
import romanize from 'romanize-korean'

romanize('안녕하세요') // annyeonghaseyo
```

### CommonJs Syntax

```javascript
// you can use in a CommonJs script as well
const romanize = require('romanize-korean')

romanize('안녕하세요') // annyeonghaseyo
```

## command-line

You can also install this module globally for command line usage

```sh
$ yarn global add romanize-korean
$ romanize-korean 안녕하세요
annyeonghaseyo
$ 
```

## Known limitations

BEWARE This module is not liaison aware because it just romanizes character-per-character.
For instance 승리 will be romanized as *seungri* while the correct pronunciation should be *seungni*.
