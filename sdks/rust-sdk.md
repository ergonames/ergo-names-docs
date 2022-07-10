# Rust SDK

Find the published SDK [here](https://crates.io/crates/ergonames).

First, we need to add our SDK to our toml file.

```
ergonames = "0.3.6"
```

Now we can import the package.

```rust
use ergonames;
```

To resolve an address from an ErgoName use the **resolve_ergoname()** function.

```rust
let name: &str = "~balb";
let address: Option<String> = ergonames::resolve_ergoname(name, None);
```

This function will either return a String or a null object.

Example result:

```
Some(3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL)
```
