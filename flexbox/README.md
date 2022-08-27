# `flex` shorthand

order: `flex-grow` `flex-shrink` `flex-basis`

default: `.flex-container { flex: 0 1 auto; }`

example: `.flex-container{ flex: 1.7 2 340px; }`

## flex-grow 
https://developer.mozilla.org/en-US/docs/Web/CSS/flex-grow

Specifies the growth factor of a flex element in its parent direction. 

The growth factor specifies how much of the remaining space within the flex container the item in question should occupy.

```css
/* <number> values */
flex-grow: 3;
flex-grow: 0.6;

/* Global values */
flex-grow: inherit | initial | revert | revert-layer | unset ;

```

## flex-shrink

https://developer.mozilla.org/en-US/docs/Web/CSS/flex-shrink

Specifies the shrinkage factor of a flex item. 

The flex **items will shrink to fill the container** according to their flex-shrink number, when the default size of the flex items is larger than that of their flex container.

```css
/* <number> values */
flex-shrink: 2;
flex-shrink: 0.6;

/* Global values */
flex-shrink: inherit | initial | revert | revert-layer | unset ;
```

## flex-basis

https://developer.mozilla.org/en-US/docs/Web/CSS/flex-basis

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
