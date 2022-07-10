# SDK Functions Overview

| Function Name     | Description                                   | Current Implementation |
| ----------------- | --------------------------------------------- | ---------------------- |
| resolve_ergoname | gets the current owner address of an ergoname | Python, JS, Rust, Scala |
| check_already_registered | checks if an ergoname is already registered | Python, JS, Rust, Scala |
| check_name_valid | checks to see if name follows ergoname minting standard | Python, JS, Rust, Scala |
| reformat_name | converts all uppercase letters to lowercase | Python, JS, Rust, Scala |
| check_name_price | returns the price to register a given ergoname | Python, JS, Rust, Scala |
| get_block_id_registered | gets the block id ergoname was registered in | Python, JS, Rust, Scala |
| get_block_registered | gets the block height ergoname was registered in | Python, JS, Rust, Scala |
| get_timestamp_registered | gets the timestamp in milliseconds since Unix epoch of block ergoname was registered in | Python, JS, Rust, Scala |
| get_date_registered | gets date of block ergoname was registered in | Python, JS, Rust, Scala |
| reverse_search | gets all the owned ergoname tokens of an address | Python, JS, Rust, Scala |
| get_total_amount_owned | returns a number of owned ergoname NFTs for a given address | Python, JS, Rust, Scala |


## Functions Example

#### resolve_ergoname()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to resolve
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let name: &str = "~balb";
let address: Option<String> = ergonames::resolve_ergoname(name, None);
```

###### Javascript
```javascript
let name = "~balb";
let address = ergonames.resolve_ergoname(name);
```

#### check_already_registered()

**Parameters:** name

- **name:** the name of the ergoname you are trying to see is already registered

###### Rust
```rust
let name: &str = "~balb";
let registerd: bool = ergonames::check_already_registered(name);
```

###### Javascript
```javascript
let name = "~balb";
let registered = ergonames.check_already_registered(name);
```

#### check_name_valid()

**Parameters:** name

- **name:** the name of the ergoname you want to see is valid

###### Rust
```rust
let name: &str = "~balb";
let valid: bool = ergonames::check_name_valid(name);
```

###### Javascript
```javascript
let name = "~balb";
let valid = ergonames.check_name_valid(name);
```

#### reformat_name()

**Parameters:** name

- **name:** the name of the ergoname you are trying to reformat

###### Rust
```rust
let name: &str = "~balb";
let reformated_name: String = ergonames::reformat_name(name);
```

###### Javascript
```javascript
let name = "~balb";
let reformated_name = ergonames.reformat_name(name);
```

#### check_name_price()

**Parameters:** name

- **name:** the name of the ergoname you are trying to get the price for

###### Rust
```rust
let name: &str = "~balb";
let price: i32 = ergonames::check_name_price(name);
```

###### Javascript
```javascript
let name = "~balb";
let price = ergonames.check_name_price(name);
```

#### get_block_id_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the block id registered in
- - **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let name: &str = "~balb";
let block_id: Option<String> = ergonames::get_block_id_registered(name, None);
```

###### Javascript
```javascript
let name = "~balb";
let block_id = ergonames.get_block_id_registered(name);
```

#### get_block_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the block number registered in
- - **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let name: &str = "~balb";
let block: Option<i32> = ergonames::get_block_registered(name, None);
```

###### Javascript
```javascript
let name = "~balb";
let block = ergonames.get_block_registered(name);
```

#### get_timestamp_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the timestamp registered
- - **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let name: &str = "~balb";
let timestamp: Option<u64> = ergonames::get_timestamp_registered(name, None);
```

###### Javascript
```javascript
let name = "~balb";
let timestamp = ergonames.get_timestamp_registered(name);
```

#### get_date_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the date registered
- - **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let name: &str = "~balb";
let date: bool = ergonames::get_date_registered(name, None);
```

###### Javascript
```javascript
let name = "~balb";
let date = ergonames.get_date_registered(name);
```

#### reverse_search()

**Parameters:** address, explorer_api

- **address:** The address you want to get the list of owned tokens for
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let address: &str = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let token_list: Option<Vec<Token>> = ergonames::reverse_search(address, None);
```

###### Javascript
```javascript
let address = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let token_list = ergonames.reverse_search(address);
```

#### get_total_amount_owned()

**Parameters:** address, explorer_api

- **address:** The address you want to get the list of owned tokens for
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

###### Rust
```rust
let address: &str = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let amount_owned: Option<u32> = ergonames::get_total_amount_owned(address, None);
```

###### Javascript
```javascript
let address = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let amount_owned = ergonames.get_total_amount_owned(address);
```