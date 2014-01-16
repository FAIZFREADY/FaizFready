* started in [jsonld.js issue](https://github.com/digitalbazaar/jsonld.js/issues/39)
* [package.json reference](https://npmjs.org/doc/json.html)

*NOTE:* we can not use `"@vocab": http://usefulinc.com/ns/doap#"` since people can add custom properties to package.json 

```js
{ "@context": {
  "doap": "http://usefulinc.com/ns/doap#",
  "url": "@id",
  "name": "doap:name",
  "description": "doap:description",
  "author": "doap:maintainter",
  "license": "doap:license", // can we map values to https://spdx.org/licenses/ ?
  ...
  },
  "homepage": {"@id": "doap:homepage", "@type": "@id"}
}
```