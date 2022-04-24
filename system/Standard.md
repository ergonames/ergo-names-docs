# Standard

### NFT Standard

Each NFT is a EIP-004 complient token on the Ergo blockchain. The supply of each token is 1, with 0 decimal places. The max supply of ErgoName NFTs is 39^20, or 66,266,211,231,824,447,117,620,880,943,201 tokens.

Encoded into each of the registers are different values:

| Register | Data Type | Data Point |
| -------- | --------- | ---------- |
| R4| Int | Royalty Percentage |
| R5 | Coll[Byte] | Name of NFT |
| R6 | Long | Payment in NanoErgs |
| R7 | Coll[Byte] | Address of minting user |

The royalty standard in register 4 is EIP-0024 complient.

### Naming Standard

- Prefix: ~
- Case: All lower case
- Numbers: Allowed
- Space: Not allowed
- Special Character: Dash, underscore, period
- Minimum Length: 1
- Maximum Length: 20

A couple examples could be:

- ~abc
- ~abc123
- ~abc_123