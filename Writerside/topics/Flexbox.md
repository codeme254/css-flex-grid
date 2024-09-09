# Flexbox

Flexbox is a new module in CSS3 that makes it easy to align elements to one another in different directions and order.  
The main idea behind Flexbox is to give the container the ability to expand and to shrink elements to best use all the available space.  
Flexbox helps us to build one-dimensional layouts.  
The element on which we use flexbox is called a ```flex container``` and all we have to do in order to create a flex container 
is to set the display property of the element to flex.  
Direct children of flex container are called ```flex items```.  
When the display property of an element is set to flex, it establishes an imaginary main axis (typically running 
horizontally from left to right) and a cross axis (typically running vertically from top to bottom), 
which dictate how the flex items are aligned and distributed within the container.

![flex container](flex-container.png)
## Flexbox properties overview
### Container properties
- **flex-direction**: specifies in which direction the main axis goes, the default is ```row```. The possible values are; ```row```,
  ```row-reverse```, ```column```, ```column-reverse```.
- **flex-wrap**: defines if flex items should wrap to a new line if there is no enough space, the default is ```nowrap```.
The possible values are; ```nowrap```, ```wrap```, ```wrap-reverse```.
- **justify-content**: they specify how the flex items will be aligned along the main axis, the default value is
  ```flex-start```. The possible values are; ```flex-start```, ```flex-end```, ```center```, ```space-between```,
  ```space-around```, ```space-evenly```.
- **align-items**: specifies how the flex items will be aligned along the cross axis, the default value is ```stretch```.
The possible values are; ```stretch```, ```flex-start```, ```flex-end```, ```center```, ```baseline```.
- **align-content**: used if there is more than one row of flex items, in this case, align-content will be used to 
control how these rows will be aligned along the cross axis, the default value is ```stretch```. The possible values are;
  ```stretch```, ```flex-start```, ```flex-end```, ```center```, ```space-between```, ```space-around```.

### Item properties
- **align-self**: aligns one individual flex item along the cross axis, the default value is ```auto```. The possible values 
are; ```auto```, ```stretch```, ```flex-start```, ```flex-end```, ```center```, ```baseline```.
- **order**: specifies the order in which one specific flex item should appear inside the container. The default value is 0, but we can pass in our own integer value.
- **flex-grow**: specifies how much an item can grow. The default value is 0, but we can pass in our own integer value.
- **flex-shrink**: specifies how much an item can shrink. The default value is 1, but we can pass in our own integer value.
- **flex-basis**: specifies the width of a flex element, the default value is ```auto``` but we can pass in our own length.