# Introduction to Media Queries with Tailwind CSS

In the previous classes you used vanilla CSS to create a responsive website. In this lesson you will use Tailwind to create a responsive website. 

## Lecture and Demonstration:

For this assignment you can use either a site you have previously created, which you will update to make it responsive, or you can choose an existing site that you will recreate as a responsive site. 

In both cases you will use Tailwind CSS. 

## What is Tailwind

Tailwind is a very popular CSS framework. Read about it here: https://tailwindcss.com

## Setup Tailwind

To use Tailwind you need to install and setup it's packages. How you do this depends on the type of project you are working with. 

**HTML/CSS/JS** 

Initilize a new npm project with:

```
npm init -y
```

Then follow the guide here: https://tailwindcss.com/docs/installation

**React**

Follow the instructions here: https://tailwindcss.com/docs/guides/create-react-app

## Intro to Tailwind

Tailwid works via utility classes that you apply to elements in your work. What does that mean? Imagine you have: 

```HTML
<p class="text-3xl font-bold underline">Hello World</p>
```

The classes added above would make the text appear as 3xl, bold, and underlined. 

What's `text-3xl`? Take a look at here: https://tailwindcss.com/docs/font-size#setting-the-font-size 

`text-3xl` makes the text `1.953rem`

`font-bold` and `underline` I'll assume are self explanatory. 

These classes all provide utility. You will be combining these utility classes together to create the styles you envision. 

This is different from defining a single class that has all of the features. Something like:

```HTML
<p class="important-text">Hello World</p>
<style>
	.important-text {
		font-size: 2rem;
		font-weight: bold;
		text-decoration: underline;
	}
</style>
```

## Tailwind classes 

Tailwind has a lot of classes. Too many to describe. 

1. Layout - Classes that help with structuring and positioning elements, such as container, grid, flex, float, clear, and display classes.
2. Typography - Classes that help with styling text and fonts, such as font, text, leading, tracking, and whitespace classes.
3. Backgrounds - Classes that help with setting background colors and images, such as bg, bg-opacity, bg-gradient-to, and bg-blur classes.
4. Borders - Classes that help with styling borders, such as border, border-opacity, border-solid, border-dashed, and border-double classes.
5. Tables - Classes that help with styling tables, such as table, table-auto, table-fixed, and table-caption classes.
6. Forms - Classes that help with styling form elements, such as form, input, select, checkbox, radio, label, and placeholder classes.
7. Effects - Classes that help with adding effects, such as shadow, opacity, transition, transform, and scale classes.
8. Interactivity - Classes that help with adding interactivity, such as hover, focus, active, and group-hover classes.
9. SVG - Classes that help with styling SVG elements, such as fill-current and stroke-current classes.
10. Accessibility - Classes that help with making content more accessible, such as sr-only, not-sr-only, focus-within, and focus-visible classes.

Note that this list is not exhaustive and there may be additional categories or classes within each category.

When using TailwindCSS when you're not sure what the class name is search the TailwindCSS site, the documentation is very good. 

https://tailwindcss.com


















The instructor will give a brief lecture on media queries and demonstrate how to use them with Tailwind CSS to create responsive layouts. They will cover topics such as:

What are media queries and why are they important for responsive design?

How do media queries work and how do you write them in CSS?

Using Tailwind CSS to simplify and speed up responsive design
Best practices for using media queries with Tailwind CSS
Challenge 1: Basic Responsive Layout

Students will be given a design brief and a basic layout to work with. Their challenge is to create a responsive layout that adapts to different screen sizes and devices using Tailwind CSS. The stretch goal is to add custom styles and design elements to make the layout more visually appealing.

## Lab Activity 1: Advanced Responsive Layout

Using Tailwind CSS, students will create a more complex and customized responsive layout. They will work individually or in pairs to experiment with different design techniques and layout options, and the stretch goal is to incorporate animation and interactivity into their design.

## Challenge 2: Responsive Design Analysis

Students will analyze the responsive design of a website of their choice, identifying the breakpoints and media queries used to adapt the layout to different screen sizes and devices. Their challenge is to present their findings and lead a discussion on the strengths and weaknesses of the design, as well as possible improvements or modifications that could be made using Tailwind CSS.

## Lab Activity 2: Customizing Tailwind CSS

In this lab activity, students will customize the Tailwind CSS framework to match their own design preferences and branding. They will experiment with different color schemes, typography, and other style options, and the stretch goal is to create a custom Tailwind CSS theme that they can use in future projects.

## Wrap-up and Homework Assignment:

In the wrap-up session, students will share their experiences and insights from the lab activities and challenges. The homework assignment will be to refine their individual designs and submit them for feedback and critique from the instructor, as well as to experiment with using media queries and Tailwind CSS in their own projects outside of class.