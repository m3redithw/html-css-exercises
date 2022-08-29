# HTML CSS Exercises

## Introduction
### ▪️ What is CSS?
- CSS stands for Cascading Style Sheets
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media
- CSS saves a lot of work. It can control the layout of multiple web pages all at once
- External stylesheets are stored in CSS files

### ▪️ CSS Solved a Big Problem
- HTML was NEVER intended to contain tags for formatting a web page!

- HTML was created to describe the content of a web page, like:

  - `<h1>This is a heading</h1>`

  - `<p>This is a paragraph.</p>`

- When tags like <font>, and color attributes were added to the HTML 3.2 specification, it started a nightmare for web developers. Development of large websites, where fonts and color information were added to every single page, became a long and expensive process.

- To solve this problem, the World Wide Web Consortium (W3C) created CSS.

- CSS removed the style formatting from the HTML page!

### ▪️ CSS Savs a Lot of Work!
- The style definitions are normally saved in external .css files.

- With an external stylesheet file, you can change the look of an entire website by changing just one file!

[Code Example](css_introduction.css)

***

## CSS Syntax
A CSS rule consists of a selector and a declaration block.
<img width="603" alt="css_syntax" src="https://user-images.githubusercontent.com/105242871/186963422-41e3d4d6-99be-47a7-8f8b-2152d396c2fc.png">

- `p` is a selector in CSS (it points to the HTML element you want to style: `<p>`).
- `color` is a property, and `red` is the property value
- `text-align` is a property, and `center` is the property value

[Code Example](css_syntax.css)

***

## CSS Selectors
CSS selectors are used to "find" (or select) the HTML elements you want to style.

We can divide CSS selectors into five categories:

- Simple selectors (select elements based on name, id, class)
- [Combinator selectors](https://www.w3schools.com/css/css_combinators.asp) (select elements based on a specific relationship between them)
- [Pseudo-class selectors](https://www.w3schools.com/css/css_pseudo_classes.asp) (select elements based on a certain TTstate)
- [Pseudo-elements selectors](https://www.w3schools.com/css/css_pseudo_elements.asp) (select and style a part of an element)
- [Attribute selectors](https://www.w3schools.com/css/css_attribute_selectors.asp) (select elements based on an attribute or attribute value)

### ▪️ The CSS element Selector
The element selector selects HTML elementsbased on the element name.

Here, all `<p>` elements on the page will be center-aligned, with a red text color:

    p {
      text-align: center;
      color: red;
    }

### ▪️ The CSS id Selector
- The id selector uses the id attribute of an HTML element to select a specific element.

- The id of an element is unique within a page, so the id selector is used to select one unique element!

- To select an element with a specific id, write a hash (#) character, followed by the id of the element.

The CSS rule below will be applied to the HTML element with id="para1": 

      #para1 {
        text-align: center;
        color: red;
      }

**Note**: An id name cannot start with a number!

### ▪️ The CSS class Selector
- The class selector selects HTML elements with a specific class attribute.

- To select elements with a specific class, write a period (.) character, followed by the class name.

In this example all HTML elements with class="center" will be red and center-aligned:

      .center {
        text-align: center;
        color: red;
      }

You can also specify that only specific HTML elements should be affected by a class.

      p.center {
        text-align: center;
        color: red;
      }

**Note**: A class name cannot start with a number!

### ▪️ The CSS Universal Selector
The universal selector (*) selects all HTML elements on the page.

The CSS rule below will affect every HTML element on the page:

      * {
        text-align: center;
        color: blue;
      }

### ▪️ The CSS Grouping Selector
The grouping selector selects all the HTML elements with the same style definitions.

Look at the following CSS code (the h1, h2, and p elements have the same style definitions):

      h1 {
        text-align: center;
        color: red;
      }

      h2 {
        text-align: center;
        color: red;
      }

      p {
        text-align: center;
        color: red;
      }

It will be better to group the selectors, to minimize the code.

To group selectors, separate each selector with a comma.

In this example we have grouped the selectors from the code above:

      h1, h2, p {
        text-align: center;
        color: red;
      }

### ▪️ All CSS Simple selectors
**Selector** |    **Example**    | **Example Description**
---|---|---
*`#id`* | #firstname | Selects the element with id="firstname"
*`.class`* | .intro | Selects all elements with class="intro"
*`element.class`* | p.intro | Selects only `<p>` elements with class="intro"
*`*`* | * | Selects all elements
*`element`* | p | 	Selects all`<p>` elements
*`element.element,..`* | div, p | 	Selects all `<div>` elements and all `<p>` elements

[Code Example](css_selector.css)

***

## How To Add CSS
### ▪️ 3 Ways to Insert CSS
- **External CSS**
  - With an external style sheet, you can change the look of an entire website by changing just one file!

  - Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

- **Internal CSS**
  - An internal style sheet may be used if one single HTML page has a unique style.

  - The internal style is defined inside the <style> element, inside the head section.

- **Inline CSS**
  - An inline style may be used to apply a unique style for a single element.

  - To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

[Code Example](insert_css.css)

***

## CSS Comments
CSS comments are not displayed in the browser, but they can help document your source code.

### ▪️ CSS Comments
Comments are used to explain the code, and may help when you edit the source code at a later date.

Comments are ignored by browsers.

A CSS comment is placed inside the `<style>` element, and starts with `/* and ends with */:`

### ▪️ HTML and CSS Comments
You can add comments to your HTML source by using the `<!--...-->` syntax.

We can use a combination of HTML and CSS comments.

[Code Example](css_comments.css)

## CSS Colors
### ▪️ CSS Color Names
In CSS, a color can be specified by using a predefined color name:

<img width="1190" alt="css_colors" src="https://user-images.githubusercontent.com/105242871/187089559-45722583-6f02-4671-9959-cda42feab5c8.png">
