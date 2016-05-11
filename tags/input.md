# input - [tag](https://github.com/GetSilverfin/sf-templates/blob/master/README.md#tags)

## `input`

Creates an input field for a [custom drop](https://github.com/GetSilverfin/sf-templates/blob/master/README.md#tags). This allows the user to enter text which can be used later on in the 

```
{% input custom.the_namespace.the_key as:currency %}
```

## Input types

To define what kind of input you want to show, you can modify the `as` parameter. Following types are currently supported:

| type       | description | what's shown as input | what's printed   | data stored |
|------------|-------------|-----------------------|------------------|-------------|-------------|
| string     | the default, just plain text                                              | <img src="../images/tags/input_string.png">        | some text  | "some text"
| text       | similar to string, but provides a bigger text field as input              | <img src="../images/tags/input_text.png">        | some text  | "some text"
| currency   | a numeric value, properly formatted with decimal and thousands separators | <img src="../images/tags/input_currency.png">        | 1.234,00   | "1234.00"
| integer    | a numeric value without decimals                                          | <img src="../images/tags/input_integer.png">        | 1.243      | "1243.00"
| percentage | a percentage value                                                        | <img src="../images/tags/input_percentage.png">        | 34,12%     | "0.3412"
| boolean    | true or false                                                             | <img src="../images/tags/input_boolean.png">        | (empty)    | "true"
| date       | a date (no time)                                                          | <img src="../images/tags/input_date.png">        | 19/09/1985 | "1985-09-19"
| account_collection | an input field that allows to select multiple accounts            | <img src="../images/tags/input_account_collection.png">        | (empty)    | "600000,610000,618200"
| file       | an input field that allows to select documents                            | <img src="../images/tags/input_file.png">        | Attachment 3 | (the actual document)
| select     | an input field to select multiple values                                  | <img src="../images/tags/input_select.png">        | the selected value | "the selected value"

## Common parameters

### `placeholder`

```
{% input custom.the_namespace.the_key placeholder:"enter name here" %}
```

This guides the user what to fill in. 


### `default`

```
{% input custom.the_namespace.the_key default:"Tony Soprano" %}
```

### `placeholder_default`

```
{% input custom.the_namespace.the_key placeholder_default:"Tony Soprano" %}
```
