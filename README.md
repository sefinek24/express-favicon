# @sefinek/express-favicon
Favicon middleware for [Express.js](https://github.com/expressjs/express).

## Installation
```bash
npm install @sefinek/express-favicon
```

## Example
```js
const express = require('express');
const favicon = require('./index.js');

const app = express();
app.use(favicon(__dirname + '/public/favicon.png'));

app.get('/', (req, res) => {
    res.send('<h1>Hello World!</h1>');
});

app.listen(3000, () => {
    console.log('Example app is ready!');
});
```

## MIT License
Copyright (c) 2023 Sefinek