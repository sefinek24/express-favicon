# @sefinek/express-favicon
Favicon middleware for [Express.js](https://github.com/expressjs/express) with [additional headers](https://github.com/sefinek24/express-favicon/blob/2b7bee22e84750b3de01448c2ec1d70b3d074aed/index.js#L25) responsible for caching the icon in the client's browser.

## Installation
```bash
npm install @sefinek/express-favicon
```

## Usage
```js
const express = require('express');
const favicon = require('@sefinek/express-favicon');

const app = express();
app.use(favicon(__dirname + '/public/favicon.png'));

app.get('/', (req, res) => {
    res.send('<h1>Hello World!</h1>');
});

app.listen(8080, () => {
    console.log('Example app is ready!');
});
```

## Example icon
![Favicon 48x48](test/favicon.png)

## MIT License
Copyright 2023 © by [Sefinek](https://sefinek.net). All Rights Reserved.