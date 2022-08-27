# CSS Flexible Box Layout

[Source: mdn web docs__](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)

[`flex`](##flex-shorthand) | [`flex-direction`](###flex-direction) | [`order`](###order) | [`flex-flow`](##the-flex-flow-shorthand)  

---

## `flex` shorthand

order: `flex-grow` `flex-shrink` `flex-basis`

default: `.flex-container { flex: 0 1 auto; }`

example: `.flex-container{ flex: 1.7 2 340px; }`

### `flex-grow`

Specifies the growth factor of a flex element in its parent direction.

The growth factor specifies how much of the remaining space within the flex container the item in question should occupy.

```css
/* <number> values */
flex-grow: 3;
flex-grow: 0.6;

/* Global values */
flex-grow: inherit | initial | revert | revert-layer | unset ;

```

### `flex-shrink`

Specifies the shrinkage factor of a flex item.

The flex **items will shrink to fill the container** according to their flex-shrink number, when the default size of the flex items is larger than that of their flex container.

```css
/* <number> values */
flex-shrink: 2;
flex-shrink: 0.6;

/* Global values */
flex-shrink: inherit | initial | revert | revert-layer | unset ;
```

### flex-basis

Initial size of a flex element. Determines the size of a content box unless otherwise specified using _box-sizing_.

```css
/* Specify <'width'> */
flex-basis: 10em | 3px | 50% | auto;

/* Intrinsic sizing keywords */
flex-basis: max-content | min-content | fit-content;

/* Automatically size based on the flex item's content */
flex-basis: content;

/* Global values */
flex-basis: inherit | initial | revert | revert-layer | unset ;
```

---

## Ordering flex items

### `flex-direction`

```css
flex-direction: row | column | row-reverse | column-reverse;
```

### `order`

Target individual items and change where they appear in the visual order.

> Items are assigned an integer that represents their group. The items are then placed in the visual order according to that integer, lowest values first. If more than one item has the same integer value, then within that group the items are laid out as per source order.

```css
order: 4; /* integer value*/
```

Flex items have a **default order value of 0**, therefore `items with an integer value greater than 0 will be displayed after` any items that have not been given an explicit order value.

You can use `negative values`. For example if you want to make one item display first and leave the order of all other items unchanged, you can give that item order of `-1`.

---

## The `flex-flow` shorthand

Direction of a flex container and its wrapping behavior. It applies to flex containers.

default: `flex-flow: row nowrap;`

```css
/* flex-flow: <'flex-direction'> */
flex-flow: row;
flex-flow: row-reverse;
flex-flow: column;
flex-flow: column-reverse;

/* flex-flow: <'flex-wrap'> */
flex-flow: nowrap;
flex-flow: wrap;
flex-flow: wrap-reverse;

/* flex-flow: <'flex-direction'> and <'flex-wrap'> */
flex-flow: row nowrap;
flex-flow: column wrap;
flex-flow: column-reverse wrap-reverse;
```
