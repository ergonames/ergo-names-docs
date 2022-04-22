# Javascript

First, we need to import the SDK.

```
npm install ergonames
```

Now that the SDK is installed, we can start integrating with the system.

To resolve an address from an ErgoName use the **resolve\_ergoname()** function.

```
let name = "~balb";
address = resolve_ergoname(name);
```

This function will either return a String or a null object.

Example result:

```
3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL
```
