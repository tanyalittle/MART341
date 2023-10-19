#### 1. Explain how web browsers function.
    Web browsers are software programs used to access the internet from a device by sending and receiving data to and from other parts of the web. The browser then translates the instructions (written in languages such as HTML, CSS, and Javascript) and renders them into visual content for the user. This information is transferred via Hypertext Transfer Protocol (HTTP).


#### 2. Define and describe DOM
    The Document Object Model (DOM) is a programming interface for web documents. It stipulates how those documents are accessed and changed. It represents the pages as nodes and objects on a tree structure so that programming languages can change the document structure, style, content, and interact with the page.


#### 3. What is the difference between HTML XML and XHTML? 
    1. HTML (Hypertext Markup Language) was the first internet language and is the foundation and structure of a page's content. 
    HTML is the most widely-used web language, has a standardized element and tagging system, and is used to render content and page structure.

    2. XML (Extensible Markup Language) is a compliment to HTML. It describes the document nodes and HTML displays them. 
    XML is stored in plan-text format, eases data transport and availability, allows for upgrading without losing data, and allows for specific elements to update without having to refresh the entire webpage.

    3. XHTML (Extensible Hypertext Markup Language) bridges the gap between HTML and XML to try to correct problems HTML causes on mobile devices in particular.
    XHTML is almost identical to HTML, its usage ensures that documents are marked-up correctly, and it has strict code requirements to make it less vulnerable to future changes; it's longer to write, but easier to maintain than HTML.



#### 4. What are the 4 elements your HTML pages need? 
    The 4 elements every HTML page you'll make will need to have:

    1. The <!DOCTYPE> declaration.
    2. The <root> element.
    3. The <head> element.
    4. The <body> element.



#### 5. What is the index.html page for? Where does it go? 
    The `index.html` page is usually the landing page (homepage) for a URL, if a file was not specified. It is first in the directory tree and websites can have multiple index files.



#### 6. Review: What are some of the best naming practices?

#### Directory
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


#### Naming Files
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