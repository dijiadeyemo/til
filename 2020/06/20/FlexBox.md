# FlexBox

**Author** : Diji

## Notes

### Introduction to FlexBox

Flexbox is a CSS module and so it involves a whole set of properties that are meant to be applied on flex containers (parent element) and flex items (childrens).
Until now, you had "block" and "inline" flow directions. Now flexbox introduce "flex-flow directions".

### Terms

* *main axis* - The main axis of a flex container is the primary axis along which flex items are laid out.
* *main-start | main-end* - The flex items are placed within the container starting from main-start and going to main-end.
* *main size* - A flex item's width or height, whichever is in the main dimension, is the item's main size.
* *cross axis* - The axis perpendicular to the main axis. Its direction depends on the main axis direction (horizontal or vertical).
* *cross-start | cross-end* - Flex lines are filled with items and placed into the container starting on the cross-start side of the flex container and going toward the cross-end side.
* *cross size* - The width or height of a flex item, whichever is in the cross dimension, is the item's cross size.

### Flex Direction

`flex-direction` defines the direction of the main-axis, defining the direction which flex items are placed in the flex container.
`flex-direction` can asume four different values:

* `row` (default)
* `row-reverse`
* `column`
* `column-reverse`

### Flex Wrap

`flex-wrap` let's you distribute flex items acrross multiple lines when these doesn't feet into the first line of the flex container.

It can asume three different values:

* `nowrap` (default)
* `wrap`
* `wrap-reverse`

### Main Axis Alignment

`justify-content` enables you to distribute free space that is left between the flex items on the main axis.

There are 5 different values that you can apply over `justify-content`

* `flex-start` (default)
* `flex-end`
* `center`
* `space-between`
* `space-around `

### Cross Axis Alignment

`align-items` defines how flex items are laid out along the cross axis on the current line.
It's like `justify-content`, but this time on the cross-axis.

There are 5 different values that you can apply over `align-items`

* `flex-start`
* `flex-end`
* `center`
* `baseline`
* `stretch` (default)

### Container Lines Alignment

`align-content` aligns the lines within a flex container when there's extra space on the cross axis.
And it only works when you have more than one line in your layout.

There are 5 different values that you can apply to `align-content`

* `flex-start`
* `flex-end`
* `center`
* `baseline`
* `stretch` (default)

### Individual Alignment

`align-self` enables you to override the alignment of a specific flex item on the cross axis.
It behaves exactly like the `align-items` property, but instead of being applied to the flex container, it is applied on flex items.

It can assume the following values:

* `auto` (default)
* `flex-start`
* `flex-end`
* `center`
* `baseline`
* `stretch`

### Order

`order` gives you the chance of changing the flex items order without having to change your HTML structure.

### Grow and Shrink

`flex-grow` enables you to fill the remaining space on the main axis changing the size of your flex items.
It can assume any positive value and the default value is 0

`flex-shrink` defines whether flex items should shrink or not.
By default it has the value 1 but it can assume the value 0 or 1

### Basis

`flex-basis` defines the default size of a flex item before the extra space is distributed.
It can assume a length (like 20% or 20em, px, etc) or a keyword. The available keywords are:

* `auto`: which is the default value.
* `content`
* `fill`
* `max-content`
* `min-content`
* `fit-content`

None of these values (except for the “auto”), are well supported yet, what makes it hard to test and to understand.

## Links

* https://www.udemy.com/course/flexbox-the-complete-guide/learn/lecture/6768872
