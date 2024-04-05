# CSS Grid

Use Grid to make flexible layouts.

## Intro 

CSS Grid is a CSS module for 2 dimensional layout. Similar to Flexbox. The difference is Flexbox is a one dimensional layout tool. Grid a is a tool for two dimensional layout. 

When should you use Flex and when should you use Grid? 

When you are trying to arrange things on a single axis, row or column, use Flex. When you are arranging things on two axis, rows and columns use Grid. 

There is some overlap. For example flex can wrap items on multiple rows or columns, and grid might be used to create a single row or column. 

## Introduction to CSS Grid:

CSS Grid is a layout system that allows you to create complex and flexible designs using a grid of rows and columns. It provides a powerful and intuitive way to arrange content on a web page, with fine-grained control over placement, sizing, and spacing.

### Basic Concepts:

In CSS Grid, you define a grid container, which is the parent element that contains the grid items. The grid container is divided into rows and columns, which are defined using the `grid-template-rows` and `grid-template-columns` properties.

Grid items are placed within the grid container using grid lines and grid tracks. Grid lines are the horizontal and vertical lines that define the edges of the rows and columns, while grid tracks are the spaces between the lines.

Read the docs! https://webkit.org/blog/7434/css-grid-layout-a-new-layout-module-for-the-web/

### Properties:

CSS Grid provides a number of properties that allow you to control the layout and positioning of grid items. Some of the most commonly used properties include:

- `grid-template-rows` and `grid-template-columns`: define the size and number of rows and columns in the grid
- `grid-template-areas`: define named areas within the grid for easier placement of items
- `gap`, `grid-column-gap`, `grid-row-gap` : set the spacing between grid tracks
- `grid-row` and `grid-column`: place an item in a specific row or column
- `grid-row-start`, `grid-row-end`, `grid-column-start`, and `grid-column-end`: place an item in a specific range of rows or columns
- `grid-area`: place an item in a specific named area

Responsive Design: One of the key benefits of CSS Grid is its _ability to create responsive designs that adapt to different screen sizes and devices_. You can use media queries and other CSS techniques to change the layout of the grid based on the screen width, rearranging the grid items as needed to provide the best user experience.

## Lab Activity Instructions:

Try this game: https://cssgridgarden.com

## In class challenge 1

Solve the challenges here: 

https://github.com/Tech-at-DU/Grid-responsive-Challenge

## In class challenge 2

**Challenge**: Solve the responsive layout challenge here: https://github.com/Tech-at-DU/responsive-web-design-challenge

You will turn in this in to GradeScope separately as it's own assignment! 

Wrap up the React Fundamentals responsive site convertion. 
