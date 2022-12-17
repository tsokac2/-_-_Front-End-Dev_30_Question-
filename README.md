<h1 align="center">Front End Dev  - Concepts</h1>

 
### What is mobile-first design?
When a designer creates a website layout specifically for mobile and adapts it to bigger screens later on.

### What is WCAG?
Web Content Accessibility Guidelines are part of a series of web accessibility guidelines.<br/>
Best and the easiest way to make a website usable for all of your customers.

### Difference between reactive and adaptive designs?
Responsive designs utilize a layout and adjust the content to fit users' screens.<br/>
Adaptive design - different fixed layouts for different user screens.

### What are fall-back fonts?
Provide backup for the fonts - if one doesn't work properly the next is a backup.<br/>


### Optimize the webpage for prints.
Use high contrast between your background and text adjust font size to improve readability.


### How to lower specificity - *"change"* ID specificity over the class?
Normal ID syntax  - ```#myId {color: red};```<br/>
Override ID syntax -  ```[id="myId"]{color: red;}```<br/>
```<p class="myClass" id="myId"></p>```


### How do you plan accessibility?
- Keyboard navigation
- Text ```alt="image content"``` HTML attribute for images
- Colour Contrast
- Element Sizes and font sizes + spacing and padding

### Example of the no-semantic elements?
`<span>` - inline element - no-semantic<br/>
`<div>` - box element  - no-semantic

## CSS

CSS Selectors?
- **id** - unique for every element
- **class** - can be applied to multiple elements
- **_*_** - selects all elements in the DOM
- `h1 {color: red;}` direct element selector

### Type of CSS selectors?
#### Descendant selector:
```div p {color: #fff;}```
```h1 span {color: #fff;}```

#### Child selector:
```div > p {color: #fff;}``` - direct child of ```div``` element

#### Adjacent siblings selector (+):
```div + p {color: #fff;}``` - directly after specific parent element

#### General siblings - ~ Tilda:
```div ~ p {color: red;}``` - next sibling of specific element

### CSS box-model?
Margin <br/>
Padding <br/>
Border <br/>
Content

### CSS viewport?
The visible area of a webpage - 1000px  = 10px = 1vh<br/>
Viewport height - 1vh = 1% of viewport height 1vh = 1%

### CSS Positions properties?

#### ```position: static;``` 
**Static** by default - always positioned according to the normal flow of the page.

#### ```position: relative;``` 
**Relative** to its normal position top, right, bottom, and left will be adjusted away from their normal position - other content will not be adjusted.

#### ```position: fixed;```
**Relative** to the viewport NO - top, right, bottom, and left - is always stays in the same place if the page is scrolled.

#### ```position: absolute;```
**Absolute** positioned to the nearest positioned ancestor or parent if no parent element then to the body - outside of the normal flow.

#### ```position: sticky;```
**Sticky** is positioned based on the user's scroll position.


### CSS pseudo-element?
A keyword is added to a selector that lets you style a specific part of the selected element(s).

Syntax - ```selector:: pseudo-element { property: value; }```

```
p:: first-line {
	color: #fff;
	font-variant: small-caps; 
	}
```
The first line in a paragraph will be red and in small caps.

### Media types in CSS?
- all		- suitable for all devices
- print 	- for print preview mode
- screen	- intended primarily for screens

### CSS3 features?
- Advance animations
- Multiple Backgrounds and Gradient
- Multiple Column layouts
- Opacity
- Rounded Corner
- Shadows
- Flexbox


### Difference between inline and inline-block elements?
```display: inline-block;``` allows to set a *width* and *height* on the element.<br/>
```display: inline;``` - can't define *width* and *height* on the element.


### Hov remove the margin in the inline-block element when kept under a div?
Assign the font size of a parent if the inline-block element to **0px** - apply font size to the inline element.


### Difference between container and container-fluid?
*Container* - provides a responsive fixed-width container<br/>
*Container-fluid* - provides a full-width container, spanning the entire width of the viewport.


### When to use !important?
Avoid using it as much as possible.
Use specificity to avoid it.
Don't use it.


### Break points in Bootstrap?
| Breakpoint |		Class infix |	Dimensions |
| ---------- | ---------------- | -------------|
| x-small		 |	xs 				| < 576px   |
| small		     |	sm  			| >= 576px |
| medium			 | md  			| >= 768px |
| large			 | lg  				| >= 992px |
| Extra large		 | xl 			| >= 1200px|
| Extra extra 	 | xxl				| >= 1400px|


### 1 REM = ? PX
REM - (root-em) - unit dictate elements' font-size relative to the size of the root element
**Font-size = 16px => 1 REM = 16 px** - in most cases


### CSS animation properties?
- animation-delay
- animation-direction
- animation-duration
- animation-fill-mode
- animation-iteration-count
- animation-name
- animation-play-state
- animation-timing-function

### CSS Preprocessors?
Sass
Less
Stylus
PostCSS

### What advantages of using SCSS over CSS?
Helps you write CSS codes easily by letting you use loops, functions, import, variables, and math operations, thus making CSS writing more powerful.


### CSS Resource(s)?
- StackOverflow
- Mozilla MDM DevDocs
- YouTube

### Cross-browser testing?
- BrowserStack
- Virtualization
- Docker

### Flexbox properties?
- flex-direction
- flex-wrap
- flex-flow
- justify-content
- align-items
- align-content


### How to manage z-index in an App?
Use Saas variables:<br/>
```
$zModal: 100;
header { z-index: $zModal; }
```


## HTML 5

### New features in HTML 5?
New tags/elements:
- ```<header>```
- ```<nav>```
- ```<section>```
- ```<aside>```

```preventDefault()``` - prevents the default behavior of HTML and events in connection with forms submitted.