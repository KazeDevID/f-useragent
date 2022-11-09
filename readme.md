# Fake User-Agent for nodejs

Just another package for generate a fake userAgent by kaze

## How to install
```bash
npm install f-useragent
```

## How to use
```javascript
const fakeUa = require('f-useragent');
console.log(fakeUa());
```

## In the real world ^o^

```javascript
const fakeUa = require('f-useragent');
const request = require('request');

var url = 'https://www.google.com.vn/search?safe=off&hl=en&q=hello';
var headers = {
  'User-Agent': fakeUa()
};
request.get({ url: url, headers: headers }, function (e, r, body) {
  console.log(r, body)
});

```
