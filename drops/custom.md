# custom - [drop](https://github.com/GetSilverfin/sf-templates/blob/master/README.md#drops)

The custom drop is a special kind of drop. It can be called on period, detail, account and company. It allows to add custom data of any kind to a specific object in Silverfin.

To reference an item in a custom drop, you always need a `namespace` and a `key`. This means you can't save information purely in a `namespace`. A custom drop with `namespace` 'the_namespace', and `key` 'the_key' on a period, would look like this:

```
  period.custom.the_namespace.the_key
```

In the custom drop you can either store a text or a dictionary. So you can store a text in `period.custom.the_namespace.the_key` or you can store a text in `period.custom.the_namespace.the_key.attribute_1` and another text in `period.custom.the_namespace.the_key.attribute_2`, effectively using `period.custom.the_namespace.the_key` as a dictionary. You can't combine both behaviours in a single custom drop.

Next to regular values, you can also store collections in a custom drop, this can be done by iterating over the namespace and then using the custom drop as a dictionary:

```liquid
{% for item in period.custom.the_namespace %}
  {{ item.some_property }}
{% endfor %}
```

To allow a user to enter information in a custom drop, it's necessary to use an [input tag](https://github.com/GetSilverfin/sf-templates/blob/master/tags/input.md). Internally the entered data will always be saved as a string and interpreted based on how it's used in the template. So data entered as a currency can be interpreted as a string.
