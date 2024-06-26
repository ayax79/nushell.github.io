---
title: dfr uppercase
categories: |
  dataframe
version: 0.92.0
dataframe: |
  Uppercase the strings in the column.
usage: |
  Uppercase the strings in the column.
feature: dataframe
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# `dfr uppercase` for [dataframe](/commands/categories/dataframe.md)

<div class='command-title'>Uppercase the strings in the column.</div>

::: warning
Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag
:::

## Signature

```> dfr uppercase {flags} ```


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Modifies strings to uppercase
```nu
> [Abc aBc abC] | dfr into-df | dfr uppercase
╭───┬─────╮
│ # │  0  │
├───┼─────┤
│ 0 │ ABC │
│ 1 │ ABC │
│ 2 │ ABC │
╰───┴─────╯

```
