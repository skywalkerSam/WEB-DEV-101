# HTML Notes

- HTML *attributes* are special words used inside the opening tag of an element to control the element's behavior. 

&emsp;

## `<!DOCTYPE html>`

- All pages should begin with `<!DOCTYPE html>`.

- `<!DOCTYPE html>` tells browsers that the document is an HTML5 document.

This special string is known as a *declaration* and ensures the browser tries to meet *industry-wide* specifications.

&emsp;

## Void Elements

- Some HTML *elements* do not have a closing tag. These are known as *void* elements.

- Here is an example of an image element which is a void element: 

```html

  <img>
```

While many code formatters like _Prettier_, will choose to include the `/` in void elements (`<img />`), the HTML spec states that the presence of the `/` "does not mark the start tag as self-closing but instead is *unnecessary* and has no effect of any kind".

&emsp;

## `<main></main>`

- The *main* element is used to represent the **main content** of the body of an HTML document.

- Content inside the *main* element should be **unique** to the document and should not be repeated in other parts of the document.

&emsp;

## `<section></section>`

- The *section* element is used to define sections in a document, such as **chapters**, **headers**, **footers**, or any other sections of the document.

- it is a *semantic element* that helps with SEO and accessibility.

&emsp;

## `<figure></figure>`

- The *figure element* represents self-contained content and will allow you to associate an image with a **caption**.

```html

<figure>
  <img src="image.jpg" alt="A description of the image">
  <figcaption>A cute image</figcaption>
</figure>
```

