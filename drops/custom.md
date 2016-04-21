# custom - [drop](https://github.com/GetSilverfin/sf-templates/blob/master/README.md#drops)

The custom drop is a special kind of drop. It can be called on period, detail, account and company. It allows to add custom data of any kind to a specific object in Silverfin.

To reference an item in a custom drop, you always need a `namespace` and a `key`. This means you can't save information purely in a `namespace`. A custom drop with `namespace` 'the_namespace', and `key` 'the_key' on a period, would look like this:

````
  period.custom.the_namspace.the_key
````
