<p align="center">
<img src="https://app.freecurrencyapi.com/img/logo/freecurrencyapi.png" width="300"/>
</p>

# freecurrencyapi-js: JS Currency Converter
Freecurrencyapi.com is a free currency API that provides realtime & historic data.
This package is a JavaScript wrapper for [freecurrencyapi.com](https://freecurrencyapi.com) that aims to make the usage of the API as easy as possible in your project.

## Installation

### npm
```shell
npm install --save @everapi/freecurrencyapi-js
```
### yarn
```shell
yarn add @everapi/freecurrencyapi-js
```

## Import

```js
import Freecurrencyapi from '@everapi/freecurrencyapi-js';
```

or use it directly in a Browser:

```html
<script src="path/to/freecurrencyapi-js/index.js"></script>
```

## Usage

Initialize the API with your API Key (get one for free at [freecurrencyapi.com](https://freecurrencyapi.com)):

```js
const freecurrencyapi = new Freecurrencyapi('YOUR-API-KEY');
```

Afterwards you can make calls to the API like this:

```js
freecurrencyapi.latest({
        base_currency: 'USD',
        currencies: 'EUR'
    }).then(response => {
        console.log(response);
    });
```

Endpoints accessible with a free account:
- `status`
- `currencies`
- `latest`
- `historical`

Find out more about our endpoints, parameters and response data structure in the [docs](https://freecurrencyapi.com/docs)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[docs]: https://freecurrencyapi.com/docs
[freecurrencyapi.com]: https://freecurrencyapi.com
