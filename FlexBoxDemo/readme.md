# Flexbox
Flexbox is a layout mechanism designed for laying out groups of items in one dimension. Learn how to use it in this module.
The Flexible Box Layout Model (flexbox) is a layout model designed for one-dimensional content.
### <b>What can you do with a flex layout? </b>
Flex layouts have the following features.

- They can display as a row, or a column.
- They respect the writing mode of the document.
- They are single line by default, but can be asked to wrap onto multiple lines.
- Items in the layout can be visually reordered, away from their order in the DOM.
- Space can be distributed inside the items, so they become bigger and smaller according to the space available in their parent.
- Space can be distributed around the items and flex lines in a wrapped layout, using the Box Alignment properties.
- The items themselves can be aligned on the cross axis.

### <b>The main axis and the cross axis </b>
The key to understanding flexbox is to understand the concept of a main axis and a cross axis. The main axis is the one set by your flex-direction property. If that is row your main axis is along the row, if it is column your main axis is along the column.

Flex items move as a group on the main axis. Remember: we've got a bunch of things and we are trying to get the best layout for them as a group.

The cross axis runs in the other direction to the main axis, so if flex-direction is row the cross axis runs along the column.