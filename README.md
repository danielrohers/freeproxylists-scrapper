# FreeProxyLists Scrapper

[![Build Status](https://travis-ci.org/rodrigogs/freeproxylists-scrapper.svg?branch=master)](https://travis-ci.org/rodrigogs/freeproxylists-scrapper)

Page scrapper that retrieves proxy server information from FreeProxyLists website.

Make sure phantomjs is installed!

> npm install freeproxylists-scrapper

```javascript
var FreeProxyLists = require('freeproxylists-scrapper');

FreeProxyLists.getPages(function (pages) {
    FreeProxyLists.crawl(pages, function (proxylist) {
        for (proxy in proxylist) {
            // You have a proxy here
        }
    });
});
```

## License

[Licence](https://github.com/rodrigogs/freeproxylists-scrapper/blob/master/LICENSE) © Rodrigo Gomes da Silva
