# [HTML](https://www.freecodecamp.org/learn/responsive-web-design-v9/) Notes

w/ freeCodeCamp.org

&nbsp;

- **Separation of concerns** is a design principle where you separate your programs into distinct sections and have each section address a separate concern.

- HTML **attributes** are special words used inside the opening tag of an element to control the element's behavior.

  - The `id` attribute adds a **unique** identifier (`#`) to an HTML element. (`#id`)

  - `class` is best used when you want to apply a set of styles to **many** elements. (`.class`)

&nbsp;

## `<!DOCTYPE html>`

it tells browsers that the document is an `HTML5` document.

- All pages should begin with `<!DOCTYPE html>`.

`Note`: This special string is known as a *declaration* and ensures the browser tries to meet *industry-wide* specifications.

&nbsp;

## Basic HTML Syntax

```html
<element attribute="value">
  inner text
</element>
```
&nbsp;

## Void Elements

Some HTML *elements* do not have a closing tag. These are known as *void* elements.

- Here is an example of an image element which is a void element: `<img>`, `<link>`, `<hr>`, `<br>`


While many code formatters like _Prettier_, will choose to include the `/` in void elements (`<img />`), the HTML spec states that the presence of the `/` "does not mark the start tag as self-closing but instead is *unnecessary* and has no effect of any kind".

&nbsp;

## `<main></main>`

The *main* element is used to represent the **main content** of the body of an HTML document.

- Content inside the *main* element should be **unique** to the document and should not be repeated in other parts of the document.

&nbsp;

## `<section></section>`

The *section* element is used to define sections in a document, such as **chapters**, **headers**, **footers**, or any other sections of the document.

- it is a semantic element that helps with *SEO* and *accessibility*.

&nbsp;

## `<div></div>`

The div element is used as a **container** to group other elements that will share a set of CSS *styles*.

- if you wanted to divide up your content into sections, then the `<section></section>` element would be more appropriate than a `div` element.

- The `section` element has semantic meaning over the `div` element which is not *semantic*.

`NOTE`: `<article></article>` elements commonly contain **multiple elements** that have **related information**.

&nbsp;

## `<figure></figure>`

The *figure element* represents self-contained content and will allow you to associate an image with a *caption*.

```html

<figure>
  <img src="image.jpg" alt="A description of the image">
  <figcaption>A cute image</figcaption>
</figure>
```

&nbsp;

## `<blockquote></blockquote>`

Blockquotes are used to indicate a section of text that is a quotation from another source. 

- Browsers typically add indentation(`&nbsp;`) and sometimes *italicize* the text.

```html
<p>Paragraph 1</p>
<p>Paragraph 2</p>
<blockquote>I think, therefore I am. (Rene Descartes)</blockquote>
<p>Paragraph 3</p>
```

&nbsp;

## HTML "entities"

- An HTML entity, or **character reference**, is a set of characters used to represent a **reserved character** in HTML.

  - if you want to write this:

    ```html
    <p>This is an <img /> element</p>
    ```
  - You have to write it like this using HTML "**entities**"

    ```html 
    <p>This is an &lt;img /&gt; element</p>
    ```
  - **Named character references** start with an *ampersand* sign (`&`) and end with a *semicolon* (`;`). 

  - **Decimal numeric references** starts with an *ampersand* sign (`&`) and *hash* symbol (`#`), followed by one or more *decimal digits*, followed by a *semicolon* (`;`).

    - &#60;

    ```html
    &#60;
    ```

    - &#169;

    ```html
    &#169;
    ```

    - &#174;

    ```html
    &#174;
    ```

  - **Hexadecimal numeric reference** starts with an *ampersand* sign (`&`), *hash* symbol (`#`), and the letter `x`. Then it is followed by one or more `ASCII hex` digits and ends with a *semicolon* (`;`).

    - &#x3C;

    ```html
    &#x3C;
    ``` 

    - &#x20AC; 
      
    ```html
    &#x20AC;
    ```

    - &#x03A9;

    ```html
    &#x03A9;
    ``` 

&nbsp;
