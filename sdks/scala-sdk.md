# Scala SDK

Find the published SDK [here](https://github.com/ergonames/ergo-names-scala-sdk/packages/1517404).

First, we need to add our SDK to our build.sbt file.

```
libraryDependencies += "TODO"
```

#### resolve_ergoname()

```scala
let name: String = "~balb";
let address: Option[String] = ergonames.resolve_ergoname(name);
```

#### check_already_registered()

```scala
let name: String = "~balb"
let registered: Booleanean = ergonames.check_already_registered(name);
```

#### check_name_valid()

```scala
let name: String = "~balb";
let valid: Boolean = ergonames.check_name_valid(name);
```

#### reformat_name()

```scala
let name: String = "~balb";
let reformated_name: String = ergonames.reformat_name(name);
```

#### check_name_price()

```scala
let name: String = "~balb";
let price: i32 = ergonames.check_name_price(name);
```

#### get_block_id_registered()

```scala
let name: String = "~balb";
let block_id: Option[String] = ergonames.get_block_id_registered(name);
```

#### get_block_registered()

```scala
let name: String = "~balb";
let block: Option[Int] = ergonames.get_block_registered(name);
```

#### get_timestamp_registered()

```scala
let name: String = "~balb";
let timestamp: Option[Long] = ergonames.get_timestamp_registered(name);
```

#### get_date_registered()

```scala
let name: String = "~balb";
let date: Boolean = ergonames.get_date_registered(name);
```

#### reverse_search()

```scala
let address: String = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let token_list: Option[Array[BalanceToken]] = ergonames.reverse_search(address);
```

#### get_total_amount_owned()

```scala
let address: String = "3WwKzFjZGrtKAV7qSCoJsZK9iJhLLrUa3uwd4yw52bVtDVv6j5TL";
let amount_owned: Option<Int> = ergonames.get_total_amount_owned(address);
```