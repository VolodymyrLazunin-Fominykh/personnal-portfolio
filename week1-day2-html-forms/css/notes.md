# Day 3 Notes - CSS Basics

## How to Add CSS

1. External: ```<link rel="stylesheet" href="css/style.css">```
2. Internal: ```<style> in <head>```
3. Inline: style="" attribute (avoid this)

## Selectors

- element { }    → All elements of that type
- .class { }     → Elements with that class
- #id { }        → Element with that ID
- element.class  → Specific element with class

## Box Model

padding → space inside element
border → edge of element
margin → space outside element

## Common Properties

- color: text color
- background-color: background color
- font-size: size of text
- font-family: font type
- width, height: dimensions

# Day 4 Notes - Flexbox

## Flex Container Properties
- display: flex; → Makes element a flex container
- flex-direction: row | column → Direction of items
- justify-content: → Horizontal alignment
  - flex-start, flex-end, center, space-between, space-around
- align-items: → Vertical alignment
  - flex-start, flex-end, center, stretch
- gap: 20px; → Space between items

## Flex Item Properties
- flex: 1; → Item takes available space
- order: 2; → Change display order

## Common Pattern
.container {
    display: flex;
    justify-content: center;  /* center horizontally */
    align-items: center;      /* center vertically */
}

# Day 5 Notes - CSS Grid

## Grid Container Properties

- display: grid; → Makes element a grid container
- grid-template-columns: 1fr 1fr 1fr; → 3 equal columns
- grid-template-columns: repeat(3, 1fr); → Same as above
- grid-template-rows: 200px auto; → Row heights
- gap: 20px; → Space between grid items

## Common Patterns
```
/*3-column layout*/
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}

/*Responsive: 2 columns on smaller screens*/
.container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}
```
## Grid vs Flexbox

- Flexbox: 1-dimensional (row OR column)
- Grid: 2-dimensional (rows AND columns)
