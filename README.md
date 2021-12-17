# multiple-ms

Convert a string to milliseconds with a simple format.

## Install

```
$ npm install multiple-ms
```

## Usage

```js
const parser = require('multiple-ms');

parser('1 hour'); // 3600000
parser('3d', true); // 3 days
parser('2w hi', { strict: true }); // undefined
parser('2h, 30m', { separator: ', ' }); // 9000000
parser('2h 30m', { separator: ', ', strict: true }); // undefined
parser('2 h', true, { language: 'es' }); // 2 horas
parser('2 horas', { language: 'en', strict: true }); // undefined
```

## License

[MIT © Cristo](./LICENSE)