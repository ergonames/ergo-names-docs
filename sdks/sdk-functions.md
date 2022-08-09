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
| check_pending_registration | checks if there are any pending registrations for an ergoname | Pythonm JS, Rust |
| available_for_registration | checks if an ergoname is available for registration | Python, JS, Rust |


## Functions Example

#### resolve_ergoname()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to resolve
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)


#### check_already_registered()

**Parameters:** name

- **name:** the name of the ergoname you are trying to see is already registered

#### check_name_valid()

**Parameters:** name

- **name:** the name of the ergoname you want to see is valid

#### reformat_name()

**Parameters:** name

- **name:** the name of the ergoname you are trying to reformat

#### check_name_price()

**Parameters:** name

- **name:** the name of the ergoname you are trying to get the price for

#### get_block_id_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the block id registered in
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

#### get_block_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the block number registered in
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

#### get_timestamp_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the timestamp registered
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

#### get_date_registered()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the date registered
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

#### reverse_search()

**Parameters:** address, explorer_api

- **address:** The address you want to get the list of owned tokens for
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)


#### get_total_amount_owned()

**Parameters:** address, explorer_api

- **address:** The address you want to get the list of owned tokens for
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

### check_pending_registration()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the pending registration for
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)

### available_for_registration()

**Parameters:** name, explorer_api

- **name:** the name of the ergoname you are trying to get the pending registration for
- **explorer_api:** The url of the explorer api is an optional parameter and is the url of thge api you querying for data (Default is **api.ergoplatform.com**)