# Python SDK

Find the published SDK [here](https://pypi.org/project/ergonames/).

First, we need to import the SDK.

```
pip install ergonames
```

#### resolve_ergoname()

```python
name = "~balb";
address = ergonames.resolve_ergoname(name);
```

#### check_already_registered()

```python
name = "~balb";
registered = ergonames.check_already_registered(name);
```

#### check_name_valid()

```python
name = "~balb";
valid = ergonames.check_name_valid(name);
```

#### reformat_name()

```python
name = "~balb";
reformated_name = ergonames.reformat_name(name);
```

#### check_name_price()

```python
name = "~balb";
price = ergonames.check_name_price(name);
```

#### get_block_id_registered()

```python
name = "~balb";
block_id = ergonames.get_block_id_registered(name);
```

#### get_block_registered()

```python
name = "~balb";
block = ergonames.get_block_registered(name);
```

#### get_timestamp_registered()

```python
name = "~balb";
timestamp = ergonames.get_timestamp_registered(name);
```

#### get_date_registered()

```python
name = "~balb";
date = ergonames.get_date_registered(name);
```

#### reverse_search()

```python
address = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
token_list = ergonames.reverse_search(address);
```

#### get_total_amount_owned()

```python
address = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
amount_owned = ergonames.get_total_amount_owned(address);
```