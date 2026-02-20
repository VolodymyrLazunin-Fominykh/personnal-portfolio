# Day 3 Notes - CSS Basics

## How to Add CSS

1. External: <link rel="stylesheet" href="css/style.css">
2. Internal: <style> in <head>
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