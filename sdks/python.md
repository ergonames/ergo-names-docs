### Python SDK currently has errors and may not be functional.

First, we need to import the SDK.

```
pip install ergonames
```

Now we can import the package.

```python
from ergonames.ergonames import resolve_ergonames
```

Now that the SDK is imported, we can start integrating with the system.

To resolve an address from an ErgoName use the **resolve\_ergoname()** function.

```python
name = "~balb";
address = resolve_ergoname(name);
```

This function will either return a String or a null object.

Example result:

```
3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL
```

