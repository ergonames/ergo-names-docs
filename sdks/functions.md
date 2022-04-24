# SDK Functions

### End-user functions

| Function Name | Description | Current Implementation |
| ------------- | ----------- | ---------------------- |
| resolve_ergoname | gets the current owner address of an ergoname | JS, Rust, Python |
| remove_quotes | removes quotation marks from a string | Rust |

### All functions

| Function Name | Description | Current Implementation |
| ------------- | ----------- | ---------------------- |
| resolve_ergoname | gets the current owner address of an ergoname | JS, Rust, Python |
| get_token_data | searches for tokens by name using the explorer API | JS, Rust, Python |
| create_token_data | calls get_token_data (possibly multiple times) to get all tokens with name | JS, Rust, Python |
| convert_token_data_to_token | converts token data retireved from API to object of type Token | JS, Rust, Python |
| get_box_address | calls explorer API and gets address of box | JS, Rust, Python |
| check_box_address | checks if address is equal to mint address | JS, Rust, Python |
| get_asset_minted_at_address | checks all assets' addresses in a token array against mint address | JS, Rust, Python |
| get_token_transaction_data | retrieves transactions for token with given id | JS, Rust, Python |
| get_max_transactions_for_token | gets total amount of transactions for token given token id | JS, Rust, Python |
| get_last_transaction | gets last transaction in list of transactions | JS, Rust, Python |
| get_box_id_from_transaction_data | gets the box id from data | JS, Rust, Python |
| reformat_name_search | changes spaces in string to %20 | JS, Rust, Python |
| remove_quotes | removes quotation marks from a string | Rust |