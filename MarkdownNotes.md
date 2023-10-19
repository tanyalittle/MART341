My Markdown practice and notes, heh.

[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

# TLDR;

*Italic*	or...   _Italic_

**Bold**   or... 	__Bold__

# Heading 1	

or...

Heading 1
=========	

## Heading 2

or...

Heading 2
---------	
Heading 2


[Link](http://a.com)	
or... 
[Link][1]
⋮
[1]: http://b.org	

Link
![Image](http://url/a.png)
or... 
![Image][1]
⋮
[1]: http://url/b.jpg	Markdown


> Blockquote	 	

* List
* List
* List

or...

- List
- List
- List


1. One
2. Two
3. Three

or...

1) One
2) Two
3) Three


Horizontal rule:

---

or...

Horizontal rule:

***


`Inline code` with backticks


```
# code block
print '3 backticks or'
print 'indent 4 spaces'
```	

or...

    # code block
    print '3 backticks or'
    print 'indent 4 spaces'








# Foobar

Foobar is a Python library for dealing with word pluralization.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install foobar
```

## Usage

```python
import foobar

# returns 'words'
foobar.pluralize('word')

# returns 'geese'
foobar.pluralize('goose')

# returns 'phenomenon'
foobar.singularize('phenomena')
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)



Thanks to [Make a README](https://www.makeareadme.com/)!





# FORMATTING

Markdown Tutorial: [commonmark.org](https://commonmark.org/help/tutorial/)





## HEADINGS:

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

Alternate Heading 1
===================

Alternate Heading 2
------------------- 

###### moving on...





## PARAGRAPHS:

#### PARAGRAPH BREAKS:
I am a paragraph. I should contain several sentences that expand on a central point or idea. If I wish to create another paragraph, I must have an empty line between myself and the beginning of the next sentence set.

I am another paragraph.
A single return does not break me.

An empty line is needed between us to fully-create another paragraph.

#### SINGLE LINE BREAKS:
For a single line break, add a backslash!\
Yeah, I'm only one space away now!

You can also end your sentence with two blank spaces!  
Now I am close without the extra backslash!





## EMPHASIS:

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Emphasis, aka italics, with *asterisks* or _underscores_.

\*Use backslash to **not** bold/italic!\*
or... \_like this\_





## LISTS:
#### ORDERED LISTS:

1. First item.
2. Second item.
3. Third item.

1) Does it, too!
2) And you can even separate them!

1. One
1. Two

and

5. Five
7. Six

22\. I don't **want** a list!

#### UNORDERED LISTS:

- An item.
- Another item.
- Yet another item.

* A new list.
* Another bit.

+ Wait, there's more!
+ And more!

#### NESTED LISTS:

To nest one list within another, indent each item in the sublist by four spaces. You can also nest other elements like paragraphs, blockquotes or code blocks.

You can mix ordered and unordered lists.

To nest a paragraph or blockquote, indent by either 4 spaces or one tab.

To nest a code block, indent by either 8 spaces or two tabs, or use a ``` code block.

* Item
    1. First Subitem
    2. Second Subitem
* Item
    - Subitem
    - Subitem
* Item

***Exercise:***

    Convert the items under "Fruit" and "Dairy" into a sublist:

* Fruit
    * Apple
    * Orange
    * Banana
* Dairy
    * Milk
    * Cheese

***Exercise:***

    Make the countries into ordered sublists:

+ World Cup 2014
    1. Germany
    2. Argentina
    3. Netherlands
+ Rugby World Cup 2015
    1. New Zealand
    2. Australia
    3. South Africa

***Exercise:***

The content under each numbered item isn’t nested properly, please fix it:

1. Ingredients

    - spaghetti
    - marinara sauce
    - salt

2. Cooking

    Bring water to boil, add a pinch of salt and spaghetti. Cook until pasta is **tender**.

3. Serve

    Drain the pasta on a plate. Add heated sauce. 

    > No man is lonely eating spaghetti; it requires so much attention.

    Bon appetit!




## LINKS:

[Course Website](https://montana-media-arts.github.io/webDesignFall2023)


#### INLINE:
Learn how to [make links in Markdown](../topic-02/markdown-links)!

#### URLS:
You can do anything at <https://html5zombo.com>

#### REFERENCE STYLE:
[Hurricane][1] Erika was the strongest and longest-lasting tropical cyclone in the 1997 Atlantic [hurricane][1] season.

[1]:https://w.wiki/qYn





## IMAGES:

Alternate (alt) text is displayed when the image can't be shown, or for the visually impaired.

Ok to leave blank but the [] is required.

![alt](https://commonmark.org/help/images/favicon.png)

No spaces between brackets.

Definition identifiers may consist of letters, numbers, spaces, and punctuation. They are not case sensitive.

The link definition can be placed anywhere after a blank line, but generally near the bottom.

The title of the image is optional.

A title provides more textual detail about what the image shows or contains.

![GitHub logo with absolute URL](https://montana-media-arts.github.io/webDesignFall2023-resources/graphics/icons/github-icon.png)

!(Git logo)[GitHub logo with relative URL](./img/github-icon.png)


Exercise: 

    Make this image appear – no need for alt text or title, leave those blank:

    ![](https://commonmark.org/help/images/favicon.png)

Exercise: 

    Add alt text of Logo and title of Creative Commons licensed to this image:

    ![Logo][1]

    [1]: https://commonmark.org/help/images/favicon.png "Creative Commons licensed"






## CODE:

To create inline code, wrap with backticks `.

To create a code block, either indent each line by 4 spaces, or place 3 backticks ``` on a line above and below the code block.

A code block or span displays every character inside exactly as it was typed, using single backticks: Inline `code` or `width=20`.

Remember, one level of indentation in a code block equals 4 spaces or one tab:

    indent 4 spaces

An indented code block continues until it reaches a line that is not indented.

3 backticks on a single line ``` ("fencing") marks the beginning and end of a code block.
This is sometimes called a “code fence”:

```
Or use 3 backticks
```

```html
width="20"
height="30"
```

**Exercise:** Format only the math in this sentence as inline code.

When `x = 3`, that means `x + 2 = 5`

**Exercise:** Format the score table as an indented code block.

Who ate the most donuts this week?

    Jeff  15
    Sam   11
    Robin  6

**Exercise:** Format this code using the code fence method.

A loop in JavaScript:
```
var i;
for (i=0; i<5; i++) {
  console.log(i);
}
```





## BLOCK QUOTES:
> First line  
> Another line
>
> > Nested line
>
> Last line





