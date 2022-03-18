# HTML CSS
Reference project that illustrates HTML, CSS, Flexbox and Bootstrap.

# Assignments
[Assignments](./assignments.md)

# Getting Started
- Clone this repo
- Install Live Server extension (VSCode)
- Right click on `index.html` and "Open with Live Server"

# Notes
HTML HyperText Markup Language is used to create Web pages and tells the browser how to display them. The purpose of CSS is to provide Web developers with a standard way to define, apply, and manage sets of style characteristics.  In other words, HTML is the data and CSS is the style.  Keeping these tasks separate is an architectual style known as the separation of concerns.

# Resources
- [W3Schools](https://www.w3schools.com/)

# HTML
- [PluralSigth HTML Fundamentals](https://app.pluralsight.com/course-player?clipId=ecbf549b-e454-4d5a-9872-367356892b14)

### HTML Semantic Elements
[HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
A semantic element clearly describes its meaning to both the browser and the developer. Examples of non-semantic elements (tells nothing about the content):
``` 
<div>
<span>
```

Examples of semantic elements (Clearly defines its content): 
```
<form>
<table>
<article>
```

HTML elements that could possibly be used by SEO:
```
<header>
<nav>
<main>
<footer>
```

# CSS
Three important concepts:
- Box Model
- CSS Selectors
- Specificity

### Box Model
- DevTools >> Elements Tab >> Scroll all the way down & click on HTML elements on left
- Margin: Outside of the HTML element
- Border: Actual border of the HTML element (the fence?)
- Padding: inside of the HTML element

### CSS Selectors
These CSS selectors are used to target HTML elements so that they can be styled:

|Example|Description|
|-----------|-----------|
|`* {}`|Universal Selector|
|`body {}`|General Selector|
|`#menu {}`|ID Selector|
|`.bookTitle {}`|Class Selector|
|`div p {}`|Descendant Selector (match any level)|
|`div > p {}`|Child Selector (match specifically)|
|`img[alt=check] {}`|Attribute Selector|
|`a:visited {}`|Psuedo Selector|

NOTE: Targeting specific HTML elements in a React App is easier because we can leverage Sassy CSS (Sass) and CSS modules.

### Specificity
Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.  In other words, specificity determines what rule sets will be applied to a target element. ProTip: Avoid `!important`
[Specificity](https://www.w3schools.com/css/css_specificity.asp)
[CSS Specificity Explained](https://youtu.be/c0kfcP_nD9E)

---

# Flexbox
[Flexbox Crash Course 2022 ](https://youtu.be/3YW65K6LcIA)
The key concept to understand when using flexbox is that there are two classes associated with "flexing", the flex container itself, and the actual item(s) inside the container.  There are properties ONLY associated with the flex container and ONLY associated with the flex item(s).  The definitions of "main axis" and "cross axis" must be undertood.  Flexbox works with block elements.

#### Flexbox Container Props
These properties ONLY apply to the flexbox container. Default direction is left-to-right (row), this is the main axis, the cross axis is 90 degrees from th main axis.

- `display`: {flex|inline-flex} Inline shrink wraps flexbox items
- `flex-direction`: {column|row} Row is the default
- `flex-wrap`: Used to specify if the flex container should wrap flex items and not squish items (squish is default)
- `flex-flow`: Shorthand for flex-direction and flex-wrap
- `justify-content`: {first baseline|center|space-between} along the main axis
- `align-items`: {flex-start|center|flex-end} Aligns the flexbox items across the CROSS axis
- `align-content`: Applies alignment accross the CROSS axis for items that wrap multiple lines (does nothing for single line flex containers) stretch is default
- `gap`: Space between flexbox items

#### Flexbox Item Props
These properties ONLY apply to the flex item(s):
- `order`: The order in which to render the flex item
- `flex-grow`: How much an item will GROW relative to the rest of the flexible items inside the same container
- `flex-shrink`: How much an item will SHRINK relative to the rest of the flexible items inside the same container
- `flex-basis`: The initial length of a flexible item 
- `flex`: Shorthand for: `flex-grow` `flex-shrink` `flex-basis`
- `align-self`: Individually change [alignment](https://getbootstrap.com/docs/5.1/utilities/flex/#align-self) for flexbox items on the cross axis, including stretch

---

#### Bootstrap Grid
TODO...


# How to Learn
What Will This Do (WWTD)?  This is a game you can play on your own to help you learn style and layout.  Try to visualize what will happen BEFORE you make a change to something.  For example:

How will the display change when 10px is changed to 20px?
```
body {
    padding: 10px; /* WWTD */
}
```
