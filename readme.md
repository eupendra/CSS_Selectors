# CSS Selectors

## What is CSS

Cascading Style Sheets.

> The name *cascading* comes from the specified priority scheme to determine which style rule applies if more than one rule matches a particular element

*Source: [Wikipedia](https://en.wikipedia.org/wiki/CSS)*

## Order of styles applied

- External CSS
- Internal CSS
- Inline CSS

## Basic selctors

- Tag Name
- Class Name
- Id
- Attribute

### TAG name

- `p` - Selects `<p>` elements
- `h1` - Selects `<h>` elements

### Class name

- `.phone` Selects elements with class `phone`

### By id

 `#phone`

### attribute

`[style="display: none;"]`

## Variations

### Multiple classes

- `.heading.dark` Selects element with these two classes
- `wikitable.sortable.plainrowheaders.jquery-tablesorter` selects elements with all these classes

### More than one elements

- `h1,h2` Selects `h1` **and** `h2` elements

### All elements

- `*` Selects **all** elements

## Advanced attribute Selections

### attribute Name and Exact Value

`[href="https://www.google.com"]`

### Has attribute, any value

`[data-country]`

### Value **begins** with

`[href^=tel]`

### Value **ends** with

`[href$=es]`

### Value **contains**

`[href*=google]`

## CSS Combinators

- descendant
- child
- adjacent sibling
- general sibling

### Descendants  (space)

 `div p` selects all `p` that are descedents (children, grandchildren, etc) of a `div` tag

### Child (>)

 `div > p` selects all `p` that are children of a `div` tag

### Adjacent Sibling (+)

 `div + p` selects ONE `p` that is immediately AFTER  `div` tag

### General Sibling (~)

 `div ~ p` selects ALL `p` that is immediately AFTER  `div` tag

## Psedo-class

### last-child

- `td:last-child` Selects every `td` that is last child of it's parent

### first-child

- `td:first-child` Selects every `td` that is first child of it's parent

### nth-child(n)

Elements that are n-th child of it's element

 link [Wikipedia Countries](http//en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population)

`table.wikitable td:nth-child(3)` Selects population column
NOTE: `table.wikitable td:nth-child(1)` doesnt select anything as the parent of `td` is `tr`, and `tr`'s first child is NOT `td` but `th`

    HINT: Think of girls and boys. A boy who was born after a girl, the boy is the second child. If you look for a first child who is a boy, you will not find anyone.
