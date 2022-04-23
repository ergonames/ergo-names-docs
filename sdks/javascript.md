# Javascript

The published SDK can be found [here](https://www.npmjs.com/package/ergonames).

First, we need to import the SDK.

```
npm install ergonames
```

Now that the SDK is installed, we can start integrating with the system.

To resolve an address from an ErgoName use the **resolve\_ergoname()** function.

```js
import { resolve_address } from "ergonames";
```

Now lets resolve the address we need.

```js
let name = "~balb";
address = resolve_ergoname(name);
```

This function will either return a String or a null object.

Example result:

```
3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL
```

