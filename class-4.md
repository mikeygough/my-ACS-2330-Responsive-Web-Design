# Introduction to Flexbox and responsive units 

This class will review flexbox and continue on to some of it's other properties, and talk about responsive units. 

## vh and vw

These are two units that can help create responsive pages. 

vh = viewport height
vw = viewport width

The viewport is the area in the browser window where your page is displayed. 

Imagine a value of 100 is 100% of the width or the height. For example if the screen is 1000px wide 50vw would be 500px. 

https://css-tricks.com/fun-viewport-units/

Use this when you need to size something based on the size of window. 

Note! vh and vw differ from % because % is based on the the parent element! Where vh and vw are based size of the view port.

## What is Flexbox

Flexbox is a layout module in CSS that provides a flexible way to arrange and align elements within a container. It allows developers to create responsive and dynamic layouts that adjust to different screen sizes and device orientations.

In Flexbox, we use a set of CSS properties to define the layout of our elements. The most important of these properties are:

1. **`display`**: flex - This property tells the browser to use the Flexbox layout mode for the selected element and its children.
2. **`flex-direction`** - This property determines the direction in which the flex items are laid out within the container. It can be set to `row`, `column`, `row-reverse`, or `column-reverse`.
3. `justify-content` - This property controls how the flex items are distributed along the main axis of the container. It can be set to `flex-start`, `flex-end`, `center`, `space-between`, `space-around`, or `space-evenly`.
4. **`align-items`** - This property controls how the flex items are aligned along the cross axis of the container. It can be set to `flex-start`, `flex-end`, `center`, `baseline`, or `stretch`.
5. **`flex-wrap`** - This property determines whether the flex items should wrap onto multiple lines or stay on a single line. It can be set to `nowrap`, `wrap`, or `wrap-reverse`.

Overall, Flexbox is a powerful tool for creating responsive and dynamic layouts, and it's an essential skill for any web developer to master.

There are a few more properties that you shouold understand. 

Here is an example. 

```HTML
<style>
	.main {
		display: flex;
		flex-direction: column;
	}
</style>
<div class="main">
	<div class="container">
		<h1>Hello</h1>
		<p>World</p>
	</div>
	<div class="footer"></div>
</div>
```

Here `div.container` and `div.footer` are "flex items" and are arrranged in a column, while `h1` and `p` are unaffected. 

Read up on flex box:

https://css-tricks.com/snippets/css/a-guide-to-flexbox/

Use those ideas to solve this game: 

https://flexboxfroggy.com

## Flex

Flex, not to be confused with flexbox, is a property that determines how a "flex item" will grow or shrink to fit the space available in its flex container. 

Try the demo here: 

https://developer.mozilla.org/en-US/docs/Web/CSS/flex

Flex determines how much of the available space an element takes up, or you could think of it as how the items divide the space between them. 

You may have noticed that when an element is display flex the child elements, the "flex items" some times get squashed to together. The flex property allows those items to decide how much of the space they will use. 

https://css-tricks.com/understanding-flex-grow-flex-shrink-and-flex-basis/

### flex-grow flex-shrink flex-basis

The flex property in CSS is used to control the flexible behavior of a container element and its child elements. It is a shorthand property that combines three individual properties: `flex-grow`, `flex-shrink`, and `flex-basis`. These three properties work together to determine how an element should grow or shrink in relation to other elements within the container. 

Flex applies to "flex items" that inside of a flex container! 

Try this example: https://www.joshwcomeau.com/css/interactive-guide-to-flexbox/

## Sticky Footer

A sticky footer is a footer that sticks to the bottom of the page **when the content doesn't reach the bottom of the window**. If the content is larger than the window the footer is below the content. 

You can implement a sticky footer in several ways. One method uses Flex. The idea is to arrange the content and the footer with flex and direction column. Set the min-height of the content to 100vh. Last set the 

## Challenge 

Apply sticky footer to the React Fundamentals tutorial. You need the footer to stick to the bottom of the page when the page is larger than the content. This will be the case on the About page and the details page. 

You will need to rearrange the HTML structure to make this work. You need the two elements. 

```HTML
<div className="App">
	<div className='App-content'>
		...
	</div>
	<Footer />
</div>
```

In App JS I have `div.App` has two child elements: `div.App-content` and `div.Footer`. You can't see it here but `<Footer />` defines a div with className "Footer". 

```CSS
.App {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.App .App-content {
  flex: 1 0 auto;
}
```

Style `div.App` with flex. Use the flex property to allow it to fill the space. 

```CSS
.Footer {
  flex-shrink: 0;
}
```

The footer needs this to allow it to sit correctly. 

**Stretch Challenge** use flex on the nav bar. 

On a wide screen the nav bar links should be arranged in a horizontal row. On the a narrow screen the two nav links should be side by side with the Ranom Spaced button below them. 

Continue the challenges from class 2. 

**Stretch Challenge** use BEM for class names. 

BEM stands for Block, Element, Modifier, and it is a popular front-end development methodology for creating reusable and maintainable code. BEM is based on the idea of breaking down user interfaces into small, modular components called blocks. Each block has its own name and encapsulated functionality, and can contain one or more elements, which are the individual parts of the block. Modifiers are used to change the appearance or behavior of blocks and elements, allowing for greater flexibility and customization. BEM is especially useful for larger projects where the codebase can quickly become unmanageable, and helps to promote consistency and clarity in code structure.

**Block**: The block is the main component of BEM, representing a self-contained piece of functionality. Blocks are usually named according to their purpose or meaning. For example, a navigation bar block might be named `nav`:

```HTML
<div class="nav">
  ...
</div>
```

In a React project the Component name might be the name of a block. 

**Element**: An element is a part of a block, representing a smaller component within the larger whole. Elements are named with a double underscore (`__`) followed by the name of the element. For example, a button element within a navigation block might be named `nav__button`:

```HTML
<div class="nav">
  <button class="nav__button">Home</button>
  ...
</div>
```

**Modifier**: Modifiers are used to modify the appearance or behavior of a block or element. Modifiers are named with a double hyphen (`--`) followed by the name of the modifier. For example, a modifier that changes the color of a button might be named `nav__button--red`:

```HTML
<div class="nav">
  <button class="nav__button nav__button--red">Home</button>
  ...
</div>
```

Using BEM in this way helps to keep the code modular and maintainable, as each component is self-contained and can be reused across the site without fear of causing conflicts or breaking styles.

Read more about BEM: https://getbem.com
