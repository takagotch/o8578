### pinyin
---
.js
https://github.com/hotoo/pinyin



#### google pinyin
http://www.google.cn/



```js
var pinyin = require("pinyin");

console.log(pinyin("xxx"));
console.log(pinyin("xxx", {
  hetaronym: true
}));
console.log(pinyin("xxx", {
  heteronym: true,
  segment: true
}));
console.log(pinyin("xxx", {
  style: pinyin.STYLE_INTIALS,
  heteronym: true
}));


const pinyin = require('pinyin');

const data = 'xxx'.split('');
const sortedData = data.sort(pinyin.compare);

const pinyin = require('pinyin');
const data = 'xxx'.split('');

const pinyinData = data.map(han => ({
  han: han,
  pinyin: pinyin(han)[0][0],
}));
const sortedData = pinyinData.sort((a, b) => {
  return a.pinyin.localeCompare(b.pinyin);
}).map(d => d.han);

```

```sh
pinyin xxx
pinyin -h

npm test
```

```
```

