---
title: "URL: host property"
short-title: host
slug: Web/API/URL/host
page-type: web-api-instance-property
browser-compat: api.URL.host
---

{{ApiRef("URL API")}} {{AvailableInWorkers}}

The **`host`** property of the {{domxref("URL")}} interface is
a string containing the host, that is the {{domxref("URL.hostname",
  "hostname")}}, and then, if the {{glossary("port")}} of the URL is nonempty, a
`':'`, followed by the {{domxref("URL.port", "port")}} of the URL.

## Value

A string.

## Examples

```js
let url = new URL("https://developer.mozilla.org/en-US/docs/Web/API/URL/host");
console.log(url.host); // "developer.mozilla.org"

url = new URL("https://developer.mozilla.org:443/en-US/docs/Web/API/URL/host");
console.log(url.host); // "developer.mozilla.org"
// The port number is not included because 443 is the scheme's default port

url = new URL("https://developer.mozilla.org:4097/en-US/docs/Web/API/URL/host");
console.log(url.host); // "developer.mozilla.org:4097"
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The {{domxref("URL")}} interface it belongs to.
