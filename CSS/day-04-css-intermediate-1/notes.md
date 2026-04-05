# Día 4 — CSS Intermediate (1/3)

## What I learned

### Advanced Selectors
- **Descendant selector** (`ul li`) — targets an element inside another, at any depth
- **Direct child selector** (`li > em`) — targets only immediate children, not deeper
- **Adjacent sibling selector** (`h1 + p`) — targets the very next sibling only
- **General sibling selector** (`h1 ~ p`) — targets all following siblings of the same level
- **Attribute selector** (`img[src="file.jpeg"]`) — targets elements with a specific attribute value; supports `^` (starts with) and `$` (ends with)

### Inheritance
- Some CSS properties (like `color`, `font-family`) are inherited by child elements automatically
- Others (like `width`, `border`) are not inherited
- `color: inherit` forces a property to inherit from the parent explicitly
- The `body` element is the parent of everything — setting `color` on it cascades down unless overridden

### Cascade & Specificity
- When two rules target the same element with equal specificity, the **last one in the file wins** (cascade)
- Specificity hierarchy: **tag (0,0,1) < class (0,1,0) < id (1,0,0)**
- An `id` always beats a class, and a class always beats a tag selector — regardless of order

## Questions


## To review
- Specificity calculation with combined selectors (e.g. `div.class#id`)
- Which CSS properties are inherited by default and which are not
