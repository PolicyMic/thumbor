# ThumborUrlBuilder

Thumbor client for Node JS

Combination of
- https://github.com/dcaramelo/ThumborUrlBuilder crypt implementation
- https://github.com/rafaelcaricio/ThumborJS build command set

Neither of these repos are updating anymore so we are maintaining our own

## Usage

```sh
# Install thumbor-url-builder module

npm install thumbor-url-builder
```

```javascript
// Declare thumbor-url-builder in JS
// Your encryption key is not required, but your link will be unsafe.

var ThumborUrlBuilder = require('thumbor-url-builder';
var thumborUrlBuilder = new ThumborUrlBuilder('MY_KEY', 'http://myserver.thumbor.com');

// Generate your url :

var thumborUrl = thumborUrlBuilder.setImagePath('00223lsvrnzeaf42.png').resize(50,50).buildUrl();
```
