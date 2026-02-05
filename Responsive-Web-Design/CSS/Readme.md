# CSS Notes

w/ freeCodeCamp.org

&nbsp;

if you think of a website as a house, `HTML` would be the foundation and framework, while `CSS` would be the paint, wallpaper, and decorations that make the house *visually appealing* and **unique***

- if `HTML` is the structure of a web page, `CSS` is what makes it *look good*.

- `CSS` works by selecting `HTML` *elements* and applying styles to them.

- `CSS` plays a vital role in creating visually appealing, responsive, and *user-friendly* websites.

Another important feature of `CSS` is its *cascading* nature, which is where the "cascading" in its name comes from (`Cascading Style Sheets`). This means that styles can be *inherited* and **overridden**, allowing for a hierarchical structure of *styling*. it allows you to build engaging web *experiences* that capture users' **attention** and enhance their interaction with web content. 

&nbsp;

## Basic Anatomy of a CSS Rule

1. A `selector`, which is a pattern used in CSS to identify and **target** specific HTML elements for styling.

    - `type` selectors
  
    - `class` selectors
  
    - `ID` selectors

2. A `declaration` block, which is a set of *styles* for a given selector, or *selectors*.

     - `property`

     - `value`

```css

selector {
  property: value;
}
```

`Note`: After each *property* name, you need to place a colon(`:`), and after each *value*, you should have a semicolon(`;`).

&nbsp;

## Units

- Pixels (`px`)
  A fixed-size unit of measurement in CSS, providing precise control over dimensions.

- Percentages (`%`)

- Viewport Units 
  
  - Viewport Width (`vw`)
  - Viewport Height (`vh`)

&nbsp;

## CSS Combinators

CSS combinators are used to define the relationship between selectors in CSS. They help in selecting elements based on their relationship to other elements, which allows for more precise and efficient styling.

- A **descendant** combinator is used to target elements matched by the second selector if they are nested within an ancestor element that matches the first selector. An ancestor can be a parent element or a parent's parent.

  ```css
  figure img {
  border: 1px solid black;
  }
  ```

- The **child** combinator (`>`) in CSS is used to select elements that are direct children of a specified parent element. 

  This combinator targets only elements with a *specific* parent, making your CSS rules more precise and preventing *unintended* styling of deeper nested elements.

  ```html
  <div class="container">
  <p>First</p>
  <div>
    <p>Second</p>
  </div>
  <div>
    <p>Third</p>
  </div>
  </div>
  ```

  - To apply styles to just the **direct child** (`<p>First</p>`) of the container class, you can use the child combinator like this:
  
  ```css
  .container > p {
  color: blue;
  }
  ```

- The **next-sibling** combinator (`+`) in CSS selects an element that immediately follows a specified sibling element. This combinator is useful when you want to apply styles to an element that directly follows another element, allowing for targeted styling based on the element's position relative to its siblings.

  ```html
  <figure>
  <img
    src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg"
    alt="A cute orange cat lying on its back."
  />
  <figcaption>A cute orange cat lying on its back.</figcaption>
  </figure>
  ```
  - Here, we have a `figure` element containing an `img` element followed by a `figcaption` element. The `figcaption` element is the immediate sibling of the `img` element.

  - if you wanted to apply a **black border** around the `figcaption` element, you can use the *next-sibling* combinator like this:

  ```css
  img + figcaption {
  border: 1px solid black;
  }
  ```

- The **subsequent-sibling** combinator (`~`) in CSS selects **all** siblings of a specified element that come after it. Unlike the *next-sibling* combinator, which targets only the immediately following sibling, the *subsequent-sibling* combinator (`~`) can target **any** siblings that follow the specified element, offering greater flexibility in *styling*.

  ```html
  <div class="container">
  <h2>Subheading</h2>
  <p>First paragraph.</p>
  <p>Second paragraph.</p>
  <p>Third paragraph.</p>
  <p>Another paragraph element</p>
  </div>
  ```
  - if you want to style **all** of the paragraph elements that come after the `h2` element, then you can use the *subsequent-sibling* combinator like this:
  
  ```css
  h2 ~ p {
  color: green;
  }
  ```
  
  - The *subsequent-sibling* combinator (`~`) targets all paragraph siblings that appear after the `h2` element, regardless of whether they are immediate siblings.

&nbsp;

## 