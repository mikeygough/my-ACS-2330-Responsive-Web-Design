# Class 1: Introduction to Responsive Web Design

# Part 1: Introduction (10 minutes)

Introduce the concept of responsive web design and its importance in modern web development.

Responsive web design is an approach to web design that aims to create websites that can adapt to different screen sizes and devices. The concept was introduced by Ethan Marcotte in 2010, who proposed designing websites to be flexible and adaptable to different devices, rather than creating separate mobile and desktop versions of a site. Since then, responsive web design has become more popular as mobile devices have become prevalent, and most modern websites are built using responsive web design techniques. With the increasing popularity of mobile devices and the introduction of new technologies, responsive web design is likely to continue to evolve and adapt to new devices and technologies in the future.

## Part 2: Group Activity (30 minutes)

Your job is to analyze these websites and identify any responsive design techniques that have been used.

To do this you will need to view the site on a desktop computer and a on a mobile device. 

Your group will present your findings to the class and discuss the strengths and weaknesses of the website's responsive design.

## Part 3: Lecture and Demonstration (20 minutes)

Responsive design is a design approach that aims to create websites that can adapt to different screen sizes and devices. The principles of responsive design involve using flexible layouts, fluid images, and media queries to ensure that the website looks good and functions well on any device.

1. **Flexible Layouts**: A flexible layout means that the design is not fixed to a specific width or height. Instead, the layout can change and adjust to the available space on the device. This is typically achieved by using relative units like percentages instead of absolute units like pixels for widths and heights. Often you will use layout properties like Flex and Grid with special units like fr (fraction.)
2. **Fluid Images**: Images are an essential part of any website, and they need to be flexible too. A fluid image can adjust its size based on the available space without losing its aspect ratio. This is typically achieved by using the max-width property in CSS.
3. **Media Queries**: Media queries are CSS rules that allow designers to target specific devices based on their screen size or other properties. By using media queries, designers can create different stylesheets that apply to different devices. For example, a designer might create a separate stylesheet for small screens like smartphones, which contains styles that are optimized for that screen size.
4. **Responsive Units**: Responsive units are units of measurement that adjust based on the screen size or device. Two commonly used responsive units are em and rem. Em is a relative unit based on the font size of the parent element, while rem is a relative unit based on the font size of the root element (typically the HTML element). By using responsive units, designers can create flexible layouts that adjust based on the user's device.

Overall, the principles of responsive design aim to create a website that provides a great user experience regardless of the user's device. By using flexible layouts, fluid images, media queries, and responsive units, designers can create websites that are optimized for different screen sizes and devices.

Demonstrate how to use media queries to create a responsive layout.

Show examples of responsive design in action and discuss best practices for optimizing responsive designs for performance.

## Part 4: Individual Activity (30 minutes)

Before writing the code to build your websites and make them responsive it is a good idea to have a visual idea of what you are going build!

The subject for this assignment will be the React Fundamentals tutorial. 

Your goal is to draw two wire frames one for the desktop version and one for a mobile version. 

Wire framing a web site involves creating a visual representation of the website's layout and structure. This representation is called a wireframe, and it's essential to creating a functional and user-friendly website. Here are some steps to help you wireframe a website:

1.Identify the website's purpose: Before you start wireframing, identify the website's purpose and goals. This will help you determine the content and features that should be included in the wireframe.
2. Determine the website's structure: The structure of the website includes the pages and sections that make up the website. Start by creating a list of the pages you want to include on your website, and then organize them into a logical structure.
3. Sketch out the wireframe: Once you have determined the website's structure, sketch out the wireframe on paper or using a digital tool. You can use a simple pen and paper, or use online wireframing tools like Figma, Adobe XD, or Sketch. A wireframe should include the page layout, including the placement of content, images, and navigation elements.
4. Keep it simple: Keep the wireframe simple and avoid getting bogged down in design details at this stage. The purpose of the wireframe is to establish the website's layout and structure, not to create a final design.
5. Test and refine: Once you have created a wireframe, test it with users or stakeholders to get feedback. Use this feedback to refine the wireframe until you have a final version that meets the website's goals and user needs.

By following these steps, you can create a clear and effective wireframe for your website. Remember that wireframing is an iterative process, so be prepared to revise and refine your wireframe as needed.



here are some tips and guidelines to help you draw a wireframe:

1. Start with a clear goal: Before starting, establish a clear goal and purpose for your wireframe. What do you want to achieve with it? What are the most important elements you need to include?
2. Keep it simple: Wireframes are not meant to be detailed designs but rather a rough sketch of the website's structure and layout. Keep it simple and focus on the overall layout and functionality of the site.
3. Use basic shapes: Use simple shapes, such as rectangles, circles, and lines, to represent the different elements of the website, including text, images, and buttons.
4. Consider content hierarchy: Pay attention to the order and placement of the content on the page. Make sure that the most important content is easily visible and accessible to the user.
5. Use a grid system: A grid system helps you create a consistent and organized layout. Use a grid system to align the different elements of the page.
6. Label your wireframe: Make sure to label your wireframe and provide a clear explanation of what each element represents. This will make it easier for others to understand your wireframe.
7. Focus on functionality: The wireframe should focus on the functionality of the website rather than the visual design. Don't worry about colors, fonts, or images at this stage.
8. Get feedback: Once you have created your wireframe, get feedback from other team members or users to see if it meets the website's goals and user needs.

By following these tips and guidelines, you can create an effective wireframe that helps you plan and design your website.

Follow these steps

1. List all of the pages
2. List the elements found on each page

## Part 5: Closing Discussion (10 minutes)

Share your wire frames. These might be in progress. 

## Homework challenge

Wire frame the React Fundamentals Tutorial (the SF Public Open Spaces Web site.) You will draw wire frames for the desktop version and a mobile version. 

The desktop version wireframes can describe the tutorial project or describe changes that you want to make to that version, it's up to you. 

The mobile version of the website doesn't exist, yet. What this looks like is up to you. **Keep in mind that the mobile site should include all of the elements from the desktop site.** You can rearrange these elements in any way that makes the most sense. Think about it from a users perspective, what would make the most sense and work best when browsing on a phone? 

You can do your work on paper, or in an application like Figma, Adobe XD, or Sketch. You can also draw your wire frames on paper. If you choose to use paper, you must draw draw neatly and not skimp on dectail! 

- Has all pages: The SFPOPOS site has three pages: Home, Details, and About
- each page includes all of it's elements. Different pages have different elements. The home page has links, random page button, search bar and list of spaces. Each space has a title, address, and image. 
- Wire frames for both desktop and mobile
- The desktop wireframe includes all of the elements
- The mobile site includes all of the elements

**Stretch Challenge** use BEM for class names. 

BEM stands for Block, Element, Modifier, and it is a popular front-end development methodology for creating reusable and maintainable code. BEM is based on the idea of breaking down user interfaces into small, modular components called blocks. Each block has its own name and encapsulated functionality, and can contain one or more elements, which are the individual parts of the block. Modifiers are used to change the appearance or behavior of blocks and elements, allowing for greater flexibility and customization. BEM is especially useful for larger projects where the codebase can quickly become unmanageable, and helps to promote consistency and clarity in code structure.

Block: The block is the main component of BEM, representing a self-contained piece of functionality. Blocks are usually named according to their purpose or meaning. For example, a navigation bar block might be named `nav`:

```HTML
<div class="nav">
  ...
</div>
```

In a React project the Component name might be the name of a block. 

Element: An element is a part of a block, representing a smaller component within the larger whole. Elements are named with a double underscore (`__`) followed by the name of the element. For example, a button element within a navigation block might be named `nav__button`:

```HTML
<div class="nav">
  <button class="nav__button">Home</button>
  ...
</div>

Modifier: Modifiers are used to modify the appearance or behavior of a block or element. Modifiers are named with a double hyphen (`--`) followed by the name of the modifier. For example, a modifier that changes the color of a button might be named `nav__button--red`:

```HTML
<div class="nav">
  <button class="nav__button nav__button--red">Home</button>
  ...
</div>

Using BEM in this way helps to keep the code modular and maintainable, as each component is self-contained and can be reused across the site without fear of causing conflicts or breaking styles.

Read more about BEM: https://getbem.com

