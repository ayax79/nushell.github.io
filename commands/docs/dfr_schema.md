---
title: dfr schema
categories: |
  dataframe
version: 0.92.0
dataframe: |
  Show schema for a dataframe.
usage: |
  Show schema for a dataframe.
feature: dataframe
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# `dfr schema` for [dataframe](/commands/categories/dataframe.md)

<div class='command-title'>Show schema for a dataframe.</div>

::: warning
Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag
:::

## Signature

```> dfr schema {flags} ```

## Flags

 -  `--datatype-list, -l`: creates a lazy dataframe


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Dataframe schema
```nu
> [[a b]; [1 "foo"] [3 "bar"]] | dfr into-df | dfr schema
╭───┬─────╮
│ a │ i64 │
│ b │ str │
╰───┴─────╯
```
