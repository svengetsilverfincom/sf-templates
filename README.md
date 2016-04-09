# Silverfin Templating Language

The Silverfin Templating Language (STL) is based on two technologies: [Liquid](https://shopify.github.io/liquid/) for logic and accessing content and [Markdown](https://daringfireball.net/projects/markdown/syntax) for styling. This guide aims to explain how these technologies can be used to create templates and texts and can be used as a reference to see where STL differs from the original technologies. Features from Liquid or Markdown that are not explicitly mentioned in this guide might work, but are not officially supported.

## Styling

### Basic styling

STL supports basic styling of text

| Style      | Syntax  | Example                      | Output
| ----------- | --------- | ------------------------------ | -------
| Bold       | `** **` | `**This is bold**`      | **This is bold**
| Italic     | `* *`   | `*This is italic*`      | *This is italic*
| Underline  | `_ _`   | `*This is underlined*`  | <img src="images/style_underlined.png" height="23" width="181">
| Bold & Italic & Underlined | `***_ _***` | `***_This is bold, italic and underlined_***` |  <img src="images/style_bold_italic_underlined.png" height="46" width="181">



### Tables

TODO


## Logic

Logic in STL is based on two important parts:

* [Drops](#drops) to access data from Silverfin, these can be considered as variables
* [Tags](#tags) to facilitate logic and more complex behaviour

### Drops

TODO

### Tags

TODO
