# Basic Layout of an HTML document:
Below is a visualization of an HTML page structure:

```
<!DOCTYPE html>
<html>

    <head>
        <title> Page title </title>
        <!-- Meta data and information about your site, not visible to visitors. -->
    </head>

    <body>
        <!-- “My Way-Cool Awesome Site!” contents, visible to visitors. See below! -->

        <h1> This is a heading </h1>
        <p> This is a paragraph. </p>
        <p> This is another paragraph. </p>
    </body>

</html>
```

***Note:*** 
Content inside `<body>` section will be displayed in browser. 
Content inside `<title>` element will be shown in browser's title bar or in page's tab.


*******************************

# What is an HTML Element?

It's defined by a start tag, some content, and an end tag:

`<tagname> Content goes here... </tagname>`

The element is everything from start tag to end tag:

`<h1> My First Heading </h1>`
`<p> My first paragraph. </p>`
`<br>`	No content; No end tag -- called an *empty element*


*******************************

# The 4 Main Document Elements:


The 4 elements every HTML page you'll make will need to have:

1. The `<!DOCTYPE>` declaration.
    - First element in HTML doc
    - Should be placed on *first line*!
    - Tells browser's processor what type of HTML doc it is
    - **NOT** an HTML tag; an instruction to browser indicating HTML page version

    `<!DOCTYPE html>`
 
2. The `<root>` element.
    - Contains all other elements & text
    - `!DOCTYPE` declares HTML version; root defines all HTML elements for page
    - It is ***necessary*** & placed outside **all** content!

``` 
<!DOCTYPE html>
<html>

</html>
```

3. The `<head>` element.
    - Container for processing info & doc metadata
    - Includes elements that may link to other files, hold author info, & passes page name to processor
    - Contains high-level info about site & ***always comes first within root***
    - Most contents not visible to site visitors; info for indexing site (i.e. search results)
    - Certain elements also dictate how page visibly looks
    *Contains the page's thoughts!*

    - Title elelment lives within head & states page title
    ***Title tag is the only required element within the head!***

```
<!DOCTYPE html>
<html>
  <head>
    <title>My Way-Cool Awesome Site</title>
    <!-- Meta data and information about your site, not visible to visitors. -->
  </head>

</html>
```


4. The `<body>` element.
    - Container for all content & data intended to be displayed on the browser's page
    - If visitor will see/have access to an element, usually in the `<body>`
    *The physical body of the site in which visitors meet, see, and interact with different elements.*

```
<!DOCTYPE html>
<html>
  <head>
    <title></title>
  </head>

  <body>
    <!-- “My Way-Cool Awesome Site!” contents, visible to visitors. -->
  </body>
</html>
```




### Example documents:

```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

#### Example Explained

- `<!DOCTYPE html>` declaration it's an HTML5 doc
- `<html>` element is root element HTML page
- `<head>` element contains meta info about HTML page
- `<title>` element specifies title -- shown in browser's title bar or in page's tab
- `<body>` element defines doc's body -- container for all visible contents: headings, paragraphs, images, hyperlinks, tables, lists, etc
- `<h1>` element defines a large heading
- `<p>` element defines a paragraph

************************





# Pages

## The Index
 - Almost all pages have an `index.html` page as their homepage, though sites can have multiple.
 - **Directory Tree:**
    ```
        .
    ├── index.html 
    ├──  css/
    │   └──  style.css
    ├──  images/
    │   ├──  photo-1.jpg
    │   └──  photo-2.jpg
    └──  pages/
        ├──  about.html
        ├──  contact.html
        └──  gallery.html
    ```



## Page URLs
 - One way to avoid long URLs is to place the page in the root of the site:
    `MART361-WebDesign/`
- This is sufficient for sites with few pages. But for sites with many, using *child directories* is preferable, as it helps with site organization.
    `https://www.baseurl.com/about.html`
    ```
        .
    ├── about.html 
    ├── index.html
    ├──  css/
    │   └──  style.css
    └──  images/
        ├──  photo-1.jpg
        └──  photo-2.jpg
    ```

- "Cleaner” looking URL? Create an additional child directory labeled `about/` and place a file saved as index.html within that directory:
    `https://www.baseurl.com/about/`
- Browsers expect to find the `index.html` so it can be left off the URL, instead ending with a directory slash `/`.
    ```
        .
    ├── index.html
    ├──  about/
    │   └──  index.html 
    ├──  css/
    │   └──  style.css
    └──  images/
        ├──  photo-1.jpg
        └──  photo-2.jpg
    ```



## Adding Content
- Anything you want a browser to render *must* be created within the `<body>` element.

### Headings in HTML
- Headings are defined with the `<h1>` to `<h6>` tags:
    `<h1> ... </h1>`

### Paragraphs
- Define paragraphs with the `<p>` tags: 
    `<p> ... </p>`

********************************

# Best Naming Practices

### Directory
- First should be the `root` folder which will contain all the elements that have to do with the website.
    - Anything **not** directly related to the website does **not** go in the `root`!
    - Each new website you work on will have its own `root` folder!
- You will **always** need to at least have an `index.html` or `index.htm` page for the website to function and it ***must be at the root level***!
- Put subpages into your page's folder!

    ##### Example Website Directory:
    - `root` folder
        - `pages` folder
            - *`page1.html`* page
            - *`page2.html`* page
            - *`page3.html`* page
        - *`index.html`* homepage
        - `images` folder
            - **`image.jpg`** image files
        - `css` folder
            - *`myStyle.css`* css file
        - `scripts` folder
            - *`script.js`* Jvascript file

*Avoid multiple subdirectories when possible; it reduces the speed of your site!*


### Naming Files
- Naming web files, folders, images, etc:
    - No spaces! Can use `_` or `-` instead!
    - No funky characters like `?`, `#`, `%`, etc!
    - All lowercase recommended, unless multiple words. Camel Casing can help make it more readable: `camelCasing.html`
    - Stick to one naming convention so you don't have to memorize every name! The web is case sensitive!!!
    - Don't start any files with numeric characters!
    - Always include an extension with file names!
        - Examples:
            ```
            Page.html
            fancy.js
            myStyles.css
            one_big_turtle.jpg
            i-love-design.html
            ```


