# period - [drop](https://github.com/GetSilverfin/sf-templates/blob/master/README.md#drops)

## `name`

`string`
The name of the period.

## `fiscal_year`

`string`
The fiscal year of this period.

## `end_date`

`date`
The date this period ends

## `start_date`

`date`
The date this period starts

## `exists`

`boolean`
Returns true when the period exists in the Silverfin database

## `calendar_years`

`array`
An array of all calendar years in the fiscal year. The information for each year is: `start_date`, `end_date`, `amount_of_days`, `amount_of_days_in_full_year`

## `month_end_dates`

`array`
An array of all the end dates of the calendar months in this fiscal year

## `year_end`

`period drop`
The period at the end of the fiscal year this period is in.

## `year_end_date`

`date`
The date of the end of the fiscal year of this period.

## `accounts`

`accounts drop`
A collection of all accounts with bookings on this period

## `reconciliations`

`reconciliations drop`
A collection of all reconciliations for this

## `people`

`people drop`
All people attached to the period (typically copied from general company level)

## `shareholders`

`people drop`
All people attached to this period that are shareholders

## `directors`

`people drop`
All people attached to this period that are directors

