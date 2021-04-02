# What is CSS

Order of styles applied:

- External CSS
- Internal CSS
- Inline CSS

## Various examples of selctors

### TAG name

Examples:
 `p`
 `h1`

### Class name

Examples

`.phone`

`wikitable.sortable.plainrowheaders.jquery-tablesorter`

### id

Example `#phone`

### attribute

`[style="display: none;"]`

## CSS Combinators

### 1. descendant selector (space)

Example `div p` selects all `p` that are descedents (children, grandchildren, etc) of a `div` tag

### 2. child selector (>)

Example `div > p` selects all `p` that are children of a `div` tag

### 3. adjacent sibling selector (+)

Example `div + p` selects ONE `p` that is immediately AFTER  `div` tag

### 4. general sibling selector (~)

Example `div + p` selects ALL `p` that is immediately AFTER  `div` tag

## Psedo-class

### nth-child(n)

Elements that are n-th child of it's element

Example link [Wikipedia Countries](https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population)

`table.wikitable td:nth-child(3)` Selects population column
NOTE: `table.wikitable td:nth-child(1)` doesnt select anything as the parent of `td` is `tr`, and `tr`'s first child is NOT `td` but `th`

    HINT: Think of girls and boys. A boy who was born after a girl, the boy is the second child. If you look for a first child who is a boy, you will not find anyone.

### last-child

### first-child


