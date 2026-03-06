# Semantic HTML

Semantics are the **meaning of words, or phrases**, in a *language*. The semantic meaning of an element refers to **what special information** that element *conveys*.

- Using proper semantic HTML will ensure the best experience for users with **assistive technology** like screen readers.

- Using correct semantic elements can improve your development experience (**DX**).

- Semantic HTML can also improve your search rankings (**SEO**).

&nbsp;

Most elements have **semantic** meaning. The `div` element is one of the very few that **does not**.

- The `header` element for defining the **header of the document, or section**.

- The navigation section element, `nav`, for sections with **navigation links**.

    ```html
    <header>
      <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Products</a>
        <a href="#">Contact</a>
      </nav>
    </header>
    ```

- The `section` element for **grouping related** information.

- The `figure` element for **illustrations** and **diagrams**.

- The `p` element is for **paragraph** of text.

&nbsp;

## Structural Hierarchy

- There can be only **one** `<h1></h1>` element per page.

- There can be **multiple** `<h2></h2>` elements.

- **Do not** skip from `h1` to `h3` directly.

- **Do not** use `<h1></h1>` to create **larger text** on your page.

  - **Use the correct structural element**, and *style* it with **CSS**. 


```html
<section>
  <h1>freeCodeCamp</h1>
  <h2>Learn Front-End Development</h2>
  <h3>Introduction to HTML</h3>
</section>
```

Finally, depending on how **incorrect** your structure is, your HTML may not even be technically valid. When this happens, **the web browser has to effectively guess what you meant to do**. And what it guesses **might not even be what you want** at all.

&nbsp;

`Note`: Using the **right hierarchy** is important for **accessibility** and **SEO**.

&nbsp;

## Presentational vs. Semantic HTML

**Presentational HTML** focuses on the **appearance** and **style** of the content.

- Used in the **early days of HTML**.

- **Deprecated** and **not recommended** anymore due to their limitations and negative impact on accessibility and maintainability.

  - `center`

    ```html
    <center>
      This text is centered.
      <p>HTML is awesome.</p>
    </center>

    <p>Another example text.</p>
    ```

  - `big`

    ```html
    <p>
      This text has a normal font size.
      <big>This text is larger.</big>
      Some other text.
    </p>
    ```

  - `font` 
    
    ```html
    <font size="7" color="blue">This text is blue and large.</font> 
    ```

&nbsp;

`Note`: While this element **still works**, you should not use it *because* the **font size and color should always be set in CSS**, not in HTML.

&nbsp;

**Semantic HTML** is now **the recommended practice**. It describes the content of the elements, so it's much **easier to read**, **understand**, and **maintain**.

- Semantic HTML **describes the content** structure, while presentational HTML **focuses on the appearance**.

&nbsp;

## 







&nbsp;





&nbsp;

