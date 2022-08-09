# SDKs

We have created 4 different SDKs for interacting with our system. Each SDK has the same function and uses the same datapoints.

All of the SDK functions can be found [here](sdk-functions.md)

### SDK List

##### Resolution SDKs

[JavaScript](resolution/javascript-sdk.md)

[Rust](resolution/rust-sdk.md)

[Python](resolution/python-sdk.md)

[Scala](resolution/scala-sdk.md)

##### Function SDKs

[JavaScript](functional/javascript-tx-lib.md)

### How It Works

The SDKs make calls to the public explorer [API endpoints](https://api.ergoplatform.com/api/v1/docs/)

The endpoints include:

- api/v1/tokens/search
- api/v1/boxes
- api/v1/assets/search/byTokenId