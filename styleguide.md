# Markdown Style Guide

## Headings

```md
# Heading h1
## Heading h2
### Heading h3
#### Heading h4
##### Heading h5
###### Heading h6
```
Note: h1 - h4 items will be automatically added to the Table of Contents.

## Emphasis

### Italics

Wrap text with a single `_` for _Italic_ text:

```md
This is _italic text_.
```

### Bold
Wrap text with double `**` for **Bold** text:

```md
This is **bold text**.
```

### Strikethrough
Wrap text with double `~~` for ~~striketrhough~~ text:

```md
This is ~~striketrhough~~ text.
```

## Links

Wrap the title in square brackets `[title]` immediately followed by the URL in `(https://example.com)`:

```md
[WordPress](https://wordpress.org/)
```

## Blockquotes

Use `>` for blockquotes, double `>>` to further indent:

```md
> Blockquote
>> Indented Blockquote
```

## Lists

### Unordered Lists

Use `-` for unordereed lists, and intent two spaces for list subitems:

```md
- List
  - List
- List
- List
```

### Ordered Lists

Use numbered items followed by a `.:

```md
1. One
2. Two
3. Three
```

## Horizontal Rules

Use `---` for a horizontal rules:
```md
---
```

## Inline Code

Wrap inline code with `\`` backticks:
```md
This is `inline code` wrapped with backticks
```

## Tables

```md
| A     | B     |
| ----- | ----- |
| Alpha | Bravo |
```

## Example Code

When documenting an example, use the markdown ``\`\`` code block to demarcate the beginning and end of the code sample:

Note: Full support for _fenced code blocks_ is not yet implemented for the handbooks, to workaround this see the shortcodes section below:

### Fenced Code Blocks

#### Javascript
```js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

#### CSS & SCSS
```css
foo {
  padding: 5px;
  margin-right: 3px;
}

.bar {
  background-color: #f00;
}
```

#### PHP
```php
$array = array(
    "foo" => "bar",
    "bar" => "foo",
);
```

#### Markdown
```md
This is _italic text_. This is **bold text**.
```

### Shortcodes

#### Javascript
```md
[javascript]
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
[/javascript]
```

#### CSS & SCSS
```md
[css]
foo {
  padding: 5px;
  margin-right: 3px;
}

.bar {
  background-color: #f00;
}
[/css]
```

#### PHP
```md
[php]
$array = array(
    "foo" => "bar",
    "bar" => "foo",
);
[/php]
```

#### Markdown
```md
[md]
This is _italic text_. This is **bold text**.
[/md]
```
Note: The `[md]` shortcode is also not currently supported.