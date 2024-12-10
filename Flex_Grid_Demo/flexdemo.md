# CSS Flexbox Layout
The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

### Flexbox Elements
To start using the Flexbox model, you need to first define a flex container.
### Parent Element (Container)
The flex container becomes flexible by setting the display property to flex:

### The flex-direction Property
The flex-direction property defines in which direction the container wants to stack the flex items.
```css
flex-direction: column; -- row
```

### The flex-wrap Property
The flex-wrap property specifies whether the flex items should wrap or not.
```css
flex-wrap: wrap;
```

### The justify-content Property
The justify-content property is used to align the flex items:
```css
justify-content: center;
```

### The align-items Property
The align-items property is used to align the flex items.
```css
align-items: center;
```

## Child Elements (Items)
The direct child elements of a flex container automatically becomes flexible (flex) items.

### The order Property
The order property specifies the order of the flex items.
```html
<div style="order: 3">1</div>
```

### The flex-grow Property
The flex-grow property specifies how much a flex item will grow relative to the rest of the flex items.
```html
<div style="flex-grow: 1">1</div>
```

### The flex-shrink Property
The flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items.
```html
<div style="flex-shrink: 0">3</div>
```

### The flex-basis Property
The flex-basis property specifies the initial length of a flex item.
```html
<div style="flex-basis: 200px">3</div>
```

### The flex Property
The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.
```html
 <div style="flex: 0 0 200px">3</div>
 ```
