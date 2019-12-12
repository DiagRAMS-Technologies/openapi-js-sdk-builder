<!--
# This file is automatically generated by a
# `metapak` module. Do NOT change it in
# place, your changes would be overriden.
-->


# @sencrop/openapi-js-sdk-builder
> Create a JavaScript SDK from an OpenAPI 3 definition


[//]: # (::contents:start)

# Usage

With a raw Node script:
```js
import { generateSDKFromOpenAPI } from 'openapi-js-sdk-builder';
import { readFileSync, writeFileSync } from 'fs';

const openAPIContents = readFileSync('openapi.json', 'utf-8');
const sdkContents = generateSDKFromOpenAPI(openAPIContents);

writeFileSync('sdk.js', sdkContents, 'utf-8');

```

You can also use the built-in [webpack loader](https://webpack.js.org/contribute/writing-a-loader/) in your frontends builds:

In `webpack.config.js`:
```js
module.exports = {
  //...
  module: {
    rules: [
      {
        test: /(\.|^)openapi.json$/,
        loader: require.resolve('openapi-js-sdk-builder'),
        type: 'javascript/auto'
      }
    ]
  }
};
```

In your code:
```js
import API from './myapi.openapi.json'

// Just use the API then
await API.getPing();

```
[//]: # (::contents:end)

# Useful resources
- [API documentation](./API.md)
- [Architecture Notes](./ARCHITECTURE.md)
- [Changelog](./CHANGELOG.md)

# License
[MIT](https://github.com/sencrop/openapi-js-sdk-builder/blob/master/LICENSE.md)


[//]: # (::contents:end)

# Useful resources
- [API documentation](./API.md)
- [Architecture Notes](./ARCHITECTURE.md)
- [Changelog](./CHANGELOG.md)

# License
[MIT](https://github.com/sencrop/@sencrop/openapi-js-sdk-builder/blob/master/LICENSE.md)
