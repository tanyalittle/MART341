# WEEK 05: HTML ELEMENTS NOTES

## Using Two-Tag Elements
- Most HTML elements consist of: 
    1. opening tag
    2. closing tag
    3. related content wrapped in-between

- General formula for an HTML element:
    - `<tagname>...content...</tagname>`

The job is simple:
- Decide on content: title, text, caption, etc.
- Wrap content in appropriate element tags: headings, paragraphs, list items, etc.
- Decide where on page each element lies: titling the page, third paragraph down, etc.

*This is part of the page structuring process.*



## Headings
- Headings are defined with `<h1>` to `<h6>` tags:
    - `<h1>...</h1>`
    - `<h1>This is a Heading 1</h1>`

- `<h1>` defines most important heading 
    - main headings
- `<h2>` are sub-headings, etc
- `<h6>` defines least important heading

***NOTE*** 
*By default, browsers display headings w/decreasing font size.*



## Paragraphs
- Devs place almost all non-heading text within paragraph element in a web doc, defined by `<p>` element:
    - `<p>...</p>`
    - `<p>This is a paragraph element.</p>`

- Any text between `<p>...</p>` belongs to same paragraph -- most common way of writing paragraphs.
- Browsers automatically add cushion above and below paragraph elements.
    - By default, browsers remove empty spaces from paragraph element blocks, spaces, and extra blank lines. 
    - Using line break, or the `<br />` tag moves the cursor to the next line within the p element.
    - Use the preformatted text element to tell a browser to render spaces and text exactly as you’ve typed:
        - `<pre>...</pre>`
        - `<pre>` usually displays contents between the element in a fixed-width font, typically used for preformatted code or text.

************************

### HTML Structure Example:
```
<html>
   <body>
      <h1>This is the Main Heading</h1>
      <p>This text might be an introduction to the rest of the page. And if the page is a long one it might be split up into several sub-headings.</p>

      <h2>This is a Sub-Heading</h2>
      <p>Many long articles have sub-headings so to help you follow the structure of what is being written. There may even be sub-sub-headings (or lower-level headings).</p>

      <h2>Another Sub-Heading</h2>
      <p>Here you can see another sub-heading followed by an associated paragraph.</p>
   </body>
</html>
```

### How Each Views:

# This is the Main Heading
This text might be an introduction to the rest of the page. And if the page is a long one it might be split up into several sub-headings.

## This is a Sub-Heading
Many long articles have sub-headings so to help you follow the structure of what is being written. There may even be sub-sub-headings (or lower-level headings).

## Another Sub-Heading
Here you can see another sub-heading followed by an associated paragraph.

*******************************

### HTML Paragraph Methods:

```
<h2>Single Paragraph</h2>
<p>
   My Bonnie lies over the ocean.

   My Bonnie lies over the sea.

   My Bonnie lies over the ocean.


   Oh,   bring back my Bonnie to me.
 </p>


<h2>Multiple Paragraphs</h2>
<p>My Bonnie lies over the ocean.</p>
<p>My Bonnie lies over the sea.</p>
<p>My Bonnie lies over the ocean.</p>
<p>Oh, bring back my Bonnie to me.</p>


<h2>Paragraph with breaks</h2>
<p>
   My Bonnie lies over the ocean.<br>

   My Bonnie lies over the sea.<br>

   My Bonnie lies over the ocean.<br>

   Oh, bring back my Bonnie to me.<br>
</p>

<h2>Preformatted Text Element</h2>
<pre>
      My Bonnie lies over the ocean.

         My Bonnie lies over the sea.

      My Bonnie lies over the ocean.


         Oh, bring back my Bonnie to me.
</pre>
```

### How each views:
**Single Paragraph**
My Bonnie lies over the ocean. My Bonnie lies over the sea. My Bonnie lies over the ocean. Oh, bring back my Bonnie to me.

**Multiple Paragraphs**
My Bonnie lies over the ocean.

My Bonnie lies over the sea.

My Bonnie lies over the ocean.

Oh, bring back my Bonnie to me.

**Paragraph with breaks**
My Bonnie lies over the ocean.
My Bonnie lies over the sea.
My Bonnie lies over the ocean.
Oh, bring back my Bonnie to me.

**Preformatted Text Element**

      My Bonnie lies over the ocean.

         My Bonnie lies over the sea.

      My Bonnie lies over the ocean.


         Oh, bring back my Bonnie to me.

*********************




## Using One-Tag Elements

- Handful of sing-tag instances known as **empty elements**.
    - General formula: `<tagname />`
- “Empty elements” only have one tag. 
- Before the closing bracket, there's often a space and forward-slash ( `/` ) character. 
- *Excellent habit to get into writing these tags in this way!*

**HTML**
```
<p>This is a paragraph. If I want additional spacing between this and the next paragraph, I can add a LINE BREAK.</p>

<br />

<p>This is another paragraph, further down the page.</p>
```



### Line Breaks

- Force a line break inside a paragraph using the break tag: `<br />`

**HTML**
```
<p>This is the first line in the paragraph.
<br />
Using a line break element, this is a separate line in the same paragraph.</p>
```

#### Example:

**HTML:**
```
<p>
This paragraph
contains a lot of <b>lines</b>
in the source code,
but the browser
ignores it.
</p>

<p>
This paragraph
contains         a lot of <b>spaces</b>
in the source         code,
but the        browser
ignores it.
</p>

<p>
This paragraph contains many lines<br />
made by using<br />
the line break tag.
</p>
```

**Result:**

This paragraph contains a lot of **lines** in the source code, but the browser ignores it.

This paragraph contains a lot of **spaces** in the source code, but the browser ignores it.

This paragraph contains many lines
made by using
the line break tag.




### Horizontal Rules

- Horizontal rule = line that spans the width of the page/browser window.
- To visually differentiate content in a doc.

**HTML**
```
<p>This is a paragraph element.</p>

<hr />

<p>This is another paragraph element.</p>
```


#### Example:
**HTML:**
```
<p>This is a full paragraph about a topic of interest. It contains information specific to that interest, and will conclude that discussion.</p>

<hr />

<p>This is another paragraph, introducing a new topic. It can be separated from the previous using a horizontal line break.</p>
```

**Result:**
This is a full paragraph about a topic of interest. It contains information specific to that interest, and will conclude that discussion.
****************************
This is another paragraph, introducing a new topic. It can be separated from the previous using a horizontal line break.



### Images

- Image tag, `<img />`, creates an empty element. 
- `src=""` tells the browser the location of the image or the URL to the file.

**HTML**
`<img src="./images/name-of-image.jpg" />`
or...
`<img src="./images/github-wave.gif" />`




### Khan Academy: Images

#### Example:
```
<!DOCTYPE html>
<html>

    <head>
        <meta charset="utf-8">
        <title>HTML: Images</title>
    </head>

    <body>

        <h1>All about rabbits!</h1>

        <img src="https://www.kasandbox.org/programming-images/animals/rabbit.png" alt="Rabbit with lop ears in barn" width="203">

        <h3>Why rabbits make great pets</h3>

        <ul>
            <li>They're furry!</li>
            <li>Great listeners!</li>
            <li>Eat all your leftover carrots!</li>
        </ul>

        <h3>Top 3 most famous rabbits</h3>

        <ol>
            <li>Bugs Bunny</li>
            <li>Easter Bunny</li>
            <li>Thumper</li>
        </ol>

        <h2>Basic info</h2>

        <p>Rabbits are little creatures with long ears and puffy tails, and they move their nose up and down in an adorable way. They eat the most orange vegetables in <em>our</em> world, and <strong>they reproduce more than any human <em>ever</em> has</strong>.</p>
        
        <h2>Songs</h2>
        
        <p>Little Bunny Foo Foo, <br>
    I don't want to see you <br>
    scooping up the field mice <br>
    and bopping them on the head!</p>

    </body>
</html>
```



*************************

## NAVIGATION: BASIC LINKS

### Internal Linking

#### Relative Linking Within Your Repository
- Remember markdown linking with an outside source and absolute URL: [discussion on absolute URLs](https://montana-media-arts.github.io/webDesignFall2023/topic-02/urls-absolute/)

- Can also link to pages on Git site using relative URLs, as long as you stay within your repo: [discussion on relative URLs](/topic-02/urls-relative/)

- Within your repo, can use either of these methods to link back to the same page. 
- One is more efficient to type and doesn’t require anything to be sent to GitHub’s servers yet.


### Page-to-Page Navigation

#### Hyperlink
- In computing, a **hyperlink**, or merely a link, refers to data that the reader can directly follow either by clicking, tapping, or hovering. 
- A hyperlink points to a whole document or a specific element within a document.

#### Hypertext
- **Hypertext** is text with hyperlinks
- The linked text = *anchor text*
- A software system used for viewing/creating Hypertext = hypertext system
- To create a hyperlink is to hyperlink (or to link). 
- A user following hyperlinks is said to navigate or browse the Hypertext. 

**NOTE** 
Link text...
- Should be specific about where the user will be going if they click a link. 
- Should **not** be simple text such as “Click Me!” 
- Correct style would dictate that the link text be:
    - description of the site
    - name, or..
    - info that informs the user


**NO** “Want to learn more? Click here!”
**YES** “See `this page about hyperlinks` to learn more.”

- Links have a straightforward tag: `<a>...</a>` 
- Any text between a hyperlink element’s tags will display as “hypertext”. 
- Traditionally blue, underlined text.
- Author must include a **hyper reference** attribute within opening tag to link to another doc: `href=""`

***NOTE***
`#` is a URL placeholder!

**HTML**
```<p>This is how you would link to <a href="https://google.com">Google's Homepage</a>.</p>```





### Khan Academy: HTML Links

#### Example:

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>HTML links</title>
    </head>
    <body>
    
        <h1>HTML: HyperText Markup Language</h1>
        
        <p>Tim Berners-Lee invented the first browser at CERN, to enable researchers to share their research with eachother.</p>
    
        <a target="_blank" href="http://home.web.cern.ch/topics/birth-web">Read more about the history of HTML
            <p>
        <img src="https://www.kasandbox.org/programming-images/misc/tim-berners-lee-webpage.png" width="300">
        <br>Image courtesy CERN    
        </p>
            
        </a>
        
        
    </body>
</html>
```

***Note:***
href = hyper reference

***********************

### Khan Academy: Internal Links

#### Example:
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>HTML internal links</title>
    </head>
    <body>
    
        <h1>HTML: HyperText Markup Language</h1>
        <ul>
            <li><a href="#web-history">History of the web</a></li>
            <li>History of HTML versions</li>
        </ul>
        <p>Tim Berners-Lee invented the first browser at CERN, to enable researchers to share their research with eachother.</p>
    
        <p>
        <img src="https://www.kasandbox.org/programming-images/misc/tim-berners-lee-webpage.png" width="200">
        <br>Image courtesy CERN    
        </p>
        
        <h2 id="web-history">History of the web</h2>
        <ul>
            <li><strong>1989: The motivation</strong>
                <p>CERN Physicist Tim Berners-Lee needed “a pool of information which could grow and evolve with the organisation and the projects it describes.”
                <br>
                <a href="http://www.w3.org/History/1989/proposal.html">Read the original proposal</a>
                </p>
            </li>
            <li>
                <strong>1989: The invention</strong>
                <p>Berners-Lee invented the World Wide Web, HTTP, and wrote the <a href="http://www.w3.org/History/19921103-hypertext/hypertext/WWW/TheProject.html">first HTML page</a>.
                </p>
            </li>
            <li>
                <strong>1993: It starts small</strong>
                <p>Berners-Lee presented the WWW at the IETF conference in a small BoF session, which is mentioned in the <a href="http://www.ietf.org/proceedings/26.pdf">proceedings</a>.</p>
            </li>
            <li>
                <strong>1993: It gets bigger!</strong>
                <p>NCSA creates the free <a href="http://www.ncsa.illinois.edu/enabling">Mosaic" browser</a>, and adds bookmarks, images, and a better UI.</p>
            </li>
            <li>
                <strong>1993+: The explosion</strong>
                <p>The number of domains increased as the internet started being <a href="http://en.wikipedia.org/wiki/History_of_the_Internet#Opening_the_network_to_commerce">used by commerce</a>.</p>
            </li>
            <li><strong>1994: The World Wide Web Consortium</strong>
                <p>Berners-Lee founds the W3C to standardize HTML for all browsers to follow.</p>
            </li>
        </ul>
        
        <h2>History of HTML versions</h2>
        <ul>
            <li>1995: HTML 2.0</li>
            <li>1997 (Jan): HTML 3.2</li>
            <li>1997 (Dec): HTML 4.0</li>
            <li>1999: HTML 4.01</li>
            <li>2004: "HTML5" is proposed by WHATWG, a new committee</li>
            <li>2008: HTML5 is adopted by W3C as a standard.</li>
        </ul>
        <p>Read more on <a href="http://en.wikipedia.org/wiki/HTML#HTML_versions_timeline">Wikipedia</a></p>
        
    </body>
</html>
```