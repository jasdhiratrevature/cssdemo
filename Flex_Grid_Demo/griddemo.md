# Grid Layout
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.


### Display Property
An HTML element becomes a grid container when its display property is set to grid or inline-grid.
```css
 display: grid;
 ```

### Grid Gaps
The spaces between each column/row are called gaps.
You can adjust the gap size by using one of the following properties:
- column-gap
- row-gap
- gap
The gap property is a shorthand property for the row-gap and the column-gap properties:
```css
 gap: 50px 100px;
 ```

### Grid Lines
- The lines between columns are called column lines.
- The lines between rows are called row lines.

## Grid Container
- To make an HTML element behave as a grid container, you have to set the display property to grid or inline-grid.
- Grid containers consist of grid items, placed inside columns and rows.

### The grid-template-columns Property
- The grid-template-columns property defines the number of columns in your grid layout, and it can define the width of each column.
- The value is a space-separated-list, where each value defines the width of the respective column.

### The grid-template-rows Property
The grid-template-rows property defines the height of each row

### The justify-content Property
The justify-content property is used to align the whole grid inside the container.

### The align-content Property
The align-content property is used to vertically align the whole grid inside the container.

## CSS Grid Item

### Child Elements (Items)
A grid container contains grid items.
By default, a container has one grid item for each column, in each row, but you can style the grid items so that they will span multiple columns and/or rows.

### The grid-column Property:
The grid-column property defines on which column(s) to place an item.
You define where the item will start, and where the item will end.
Make "item1" start on column 1 and end before column 5:

```css
.item1 {
  grid-column: 1 / 5;
}
```

### The grid-row Property:
The grid-row property defines on which row to place an item.
You define where the item will start, and where the item will end.

Make "item1" start on row-line 1 and end on row-line 4:
```css
.item1 {
  grid-row: 1 / 4;
}
```
