# Rust SDK

Find the published SDK [here](https://crates.io/crates/ergonames).

First, we need to add our SDK to our toml file.

```
ergonames = "0.3.6"
```

#### resolve_ergoname()

```rust
let name: &str = "~balb";
let address: Option<String> = ergonames::resolve_ergoname(name, None);
```

#### check_already_registered()

```rust
let name: &str = "~balb";
let registerd: bool = ergonames::check_already_registered(name);
```

#### check_name_valid()

```rust
let name: &str = "~balb";
let valid: bool = ergonames::check_name_valid(name);
```

#### reformat_name()

```rust
let name: &str = "~balb";
let reformated_name: String = ergonames::reformat_name(name);
```

#### check_name_price()

```rust
let name: &str = "~balb";
let price: i32 = ergonames::check_name_price(name);
```

#### get_block_id_registered()

```rust
let name: &str = "~balb";
let block_id: Option<String> = ergonames::get_block_id_registered(name, None);
```

#### get_block_registered()

```rust
let name: &str = "~balb";
let block: Option<i32> = ergonames::get_block_registered(name, None);
```

#### get_timestamp_registered()

```rust
let name: &str = "~balb";
let timestamp: Option<u64> = ergonames::get_timestamp_registered(name, None);
```

#### get_date_registered()

```rust
let name: &str = "~balb";
let date: bool = ergonames::get_date_registered(name, None);
```

#### reverse_search()

```rust
let address: &str = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let token_list: Option<Vec<Token>> = ergonames::reverse_search(address, None);
```

#### get_total_amount_owned()

```rust
let address: &str = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let amount_owned: Option<u32> = ergonames::get_total_amount_owned(address, None);
```