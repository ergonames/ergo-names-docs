# Javascript SDK

Find the published SDK [here](https://www.npmjs.com/package/ergonames).

First, we need to import the SDK.

```
npm install ergonames
```

#### resolve_ergoname()

```javascript
let name = "~balb";
let address = ergonames.resolve_ergoname(name);
```

#### check_already_registered()

```javascript
let name = "~balb";
let registered = ergonames.check_already_registered(name);
```

#### check_name_valid()

```javascript
let name = "~balb";
let valid = ergonames.check_name_valid(name);
```

#### reformat_name()

```javascript
let name = "~balb";
let reformated_name = ergonames.reformat_name(name);
```

#### check_name_price()

```javascript
let name = "~balb";
let price = ergonames.check_name_price(name);
```

#### get_block_id_registered()

```javascript
let name = "~balb";
let block_id = ergonames.get_block_id_registered(name);
```

#### get_block_registered()

```javascript
let name = "~balb";
let block = ergonames.get_block_registered(name);
```

#### get_timestamp_registered()

```javascript
let name = "~balb";
let timestamp = ergonames.get_timestamp_registered(name);
```

#### get_date_registered()

```javascript
let name = "~balb";
let date = ergonames.get_date_registered(name);
```

#### reverse_search()

```javascript
let address = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let token_list = ergonames.reverse_search(address);
```

#### get_total_amount_owned()

```javascript
let address = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let amount_owned = ergonames.get_total_amount_owned(address);
```