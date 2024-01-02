# CSS

While HTML is the structure of the building, CSS is the paint that makes the house pretty.
CSS stylesheets are applied in order in which they follow each other
Inline CSS takes precedence over any other css stylesheet.
CSS is applied from top to bottom therefore the last rule of a specific element is applied.
p{
color:purple;
}
p-> selector
color:purple; -> declaration
color->property
purple->propery value

# CSS Validation

CSS Validation Service
http://jigsaw.w3.org/css-validator/

# SELECTORS PRECEDENCE

use the specificity calculator to determine the selectors precedence

ID -> CLASSES -> Element Selectors

# INHERITANCE

Inheritance is when another element inherits the settings or properties from its parent element
Properties that are inherited include: fonts and typograhpy
Form elements do not inherit typography

# COLORS

Color Pallet Picker Tool and Color Contrast Checker:
https://coolors.co

Color Contrast Checker:
https://webaim.org

# UNIT SIZES

The default font size is 16px

Examples of Unit Sizes:

1. Absolute Length Units:
   Pixels -> px
   Example:
   font-size:20px;
   border: 2px solid black;

2. Relative Length Units:
   1.REM -> Root Element
   Rem ->relates to the font size of the root element
   1 rem is basically the root fontsize which is mostly 16px
   1rem = 16px
   2rem = 32px
   Example:
   p{
   font-size:
   }
   2.EM-> relates to the fontsize of the parent element
   1em = parent font size 3. VH and VW
   Example:
   main{
   height:100vh;
   }

3. Numbers, Length and Percentages:
   percentages are also relative to other qauntity
   Example:
   width: 100%;

Places to use absolute values like pixels:
.borders
Places to use REMS:
.typography
Places to use Ems:
.margin and paddings and buttons
Places to use Percentages:
.widths

# BLOCK ELEMENTS

Block elements have 100% width of whats available to them by default and they also stack on top of each other.
They also have some default margin.

# INLINE ELEMENTS

you cant apply margin and height to inline elements
and when you apply padding to them they overlap

# INLINE-BLOCK

inline-block elements dont create new lines,they stay inline but you can apply height, padding and margin

# MEDIA QUERIES

Syntax:
@media media type and (condition:breakpoint){
//CSS RULES
}

@media screen and (min-width:breakpoint) {
//CSS RULES
}

Media Queries Conditions:
min-width
max-width
min-aspect-ratio
orientation

min-width-> the styles specified with apply upto the specified width.
max-width->starting from.The styles specified will start from the specified width.

### Common Media Query Breakpoints

| BreakPoint         | Description               |
| ------------------ | ------------------------- |
| < 481px            | Mobile Devices            |
| 481px -> 768px     | ipads, tablets            |
| 769px -> 104px     | small screens and laptops |
| 1025px -> 1200px   | Desktops, large screens   |
| 1201px and greater | Extra large screens, Tvs  |

### Bootstrap breakpoints

| BreakPoint | Description |
| ---------- | ----------- |
| < 576px    | xs          |
| >=576px    | small       |
| >=768px    | medium      |
| >=992px    | large       |
| >=1200px   | xl          |
| >=1400px   | 2xl         |

### Tailwind breakpoints

| BreakPoint | Description |
| ---------- | ----------- |
| < 640px    | xs          |
| >=640px    | small       |
| >=768px    | medium      |
| >=1024px   | large       |
| >=1280px   | xl          |
| >=1536px   | 2xl         |
