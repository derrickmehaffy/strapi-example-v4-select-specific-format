# example to select a specific format object from the formats json field

```js
const qs = require('qs');

const query = qs.stringify({
  populate: {
    mediaField: {
      fields: ['formats'],
      populate: {
        fields: ['thumbnail'],
      }
    },
  }
}, {
  encodeValuesOnly: true,
});


console.log('\n' + query)
```
