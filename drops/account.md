# account - [drop](https://github.com/GetSilverfin/sf-templates/blob/master/README.md#drops)

## `name`

`string`
Name of the account

## `number`

`string`
Number/code of the account

## `link`

`string`
Concatenation of the number and name of the account, when shown in the Silverfin interface, this is also a link to the account

## `value`

`decimal`
The value for the account in this period

## `debet_value`

`decimal`
The sum of all debet transactions for the account in this period

## `credit_value`

`decimal`
The sum of all credit transactions for the account in this period

## `details_sum`

`decimal`
The sum of all values of the details for the account in this period

## `transferred_opening_value`

`decimal`
This is the value transferred by Silverfin from the previous year. This is only relevant for balance accounts and is only different from 0 when Silverfin did the transfer itself

## `opening_value`

`decimal`
The value for this account in the last period of the previous book year. If the last period of the previous book year does not exist in Silverfin, this will be 0

## `asset_or_expense`

`boolean`
True when the account is an asset or an expense

## `liability_or_income`

`boolean`
True when the account is a liability or income

## `is_account`

`boolean`
Always true

## `preferred_orientation`
`portrait` or `landscape`
String representing the preferred orientation for the template of the account, depending on the content

## `transactions`

`[transaction]`
All transactions of the book year up till this period for the account

## `details`

`[detail]`
All details for the account in this period

## `results`

`[]`
An array of all named results for the account in this period

## `custom`

`custom drop`
A way to attach custom information to the account for the current period
