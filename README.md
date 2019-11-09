# Privacy API

Privacy API is an NPM Package for for communicating with the privacy.com API

## Installation

Use the package manager [npm](https://www.npmjs.com/get-npm) to install `privacy-api`.

```bash
npm install privacy-api
```

## Usage

Responses are returned as standard [axios responses](https://github.com/axios/axios#response-schema)

```javascript
const privacy = require('privacy-api');
let privacy_api = new privacy(<API-KEY>);
let response = await privacy_api.list_cards();

console.log(response.data);
```

### Available Functions

 - list_cards(page, page_size, begin, end, card_token) &#8594; Lists all available cards for this user
   - https://developer.privacy.com/docs#endpoints-list-cards

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)