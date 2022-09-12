# Token Standard

### NFT Standard

Each NFT is a EIP-004 complient token on the Ergo blockchain. The supply of each token is 1, with 0 decimal places. The max supply of ErgoName NFTs is 39^20, or 66,266,211,231,824,447,117,620,880,943,201 tokens.

Encoded into each of the registers are different values:

| Register | Data Type | Data Point |
| -------- | --------- | ---------- |
| R4 | Coll[Byte] | Name of Token |
| R5 | Coll[Byte] | Description of Token |
| R6 | Int | Number of Decimals |
| R7 | Coll[Byte] | 0e020101 to specify Picture NFT |
| R8 | Coll[Byte] | SHA-256 Hash of Image File |
| R9 | Coll[Byte] | SVG Image Encoded |

The royalty standard in register 4 is EIP-0024 compliant.

### Naming Standard

- Prefix: ~
- Case: All lower case
- Numbers: Allowed
- Space: Not allowed
- Special Character: Dash, underscore, period
- Minimum Length: 1
- Maximum Length: 20

A couple of examples could be:

- ~abc
- ~abc123
- ~abc_123