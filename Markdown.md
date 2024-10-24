# The Markdown markup language ![](./assets/Markdown-66x40.png)

Markdown is a lightweight markup language for creating formatted text using a plain-text editor.  It was created by John Gruber and Aaron Swartz in 2004.  It has become a popular format for writing documentation for code.

*   A *markup language* describes the appearance of a rich document only using plain text.
    *   A *rich document* presents text using different fonts, colors and styles, and possibly includes images and other multi-media elements
        *   e.g. a Word document or a webpage
*   HTML is a common markup language, but is hard to read in its raw form
    *   Markdown aims to produce documents that are readable to humans in their raw form, and simple to convert into HTML.

This document introduces only the most basic features of Markdown.  More is possible, but is left for you to discover.

You will notice that content is duplicated in the sections that follow.  After a Markdown feature is demonstrated, it is followed by a text block that shows what the Markdown source code looks like.



## Table of Contents
*   [Headers](#headers)
*   [Paragraphs](#paragraphs)
*   [Pre-formatted Code Blocks](#pre-formatted-code-blocks)
*   [Tables](#tables)
*   [Lists](#lists)
*   [Checkboxes](#checkboxes)
*   [Hyperlinks](#hyperlinks)
*   [Images](#images)
*   [Markdown Hints](#markdown-hints)
*   [More resources](#more-resources)



## Headers

*   Begin a line of text with consecutive `#` to introduce a header.
*   Markdown defines six (6) levels of header, using from 1 to 6 `#`'s
    *   Lower level headers are presented in smaller fonts

# This is a level 1 Header
## This is a level 2 Header
### This is a level 3 Header
#### This is a level 4 Header
##### This is a level 5 Header
###### This is a level 6 Header

```
# This is a level 1 Header
## This is a level 2 Header
### This is a level 3 Header
#### This is a level 4 Header
##### This is a level 5 Header
###### This is a level 6 Header
```



## Paragraphs

Consecutive lines of text are formed into paragraphs.
Lines of text in paragraphs can be as long
or as short
as
you
want.

Indentation
    is not preserved
        by paragraphs.
            The text is automatically 
                re-flowed
            to fit
        the width
    of the
window.

Separate paragraphs from one another with blank lines.

Inside paragraphs you can write **bold text** by surrounding words with two asterisks, `**`.
_Italicized text_ is surrounded by single underlines `_`.
~~Struck through text~~ is surrounded by double tildes `~~`.
A `code span` is created by surrounding text with a back-tick `` ` ``
(**_Hint_**: back-tick shares the same key as `~`).

```
Consecutive lines of text are formed into paragraphs.
Lines of text in paragraphs can be as long
or as short
as
you
want.

Indentation
    is not preserved
        by paragraphs.
            The text is automatically 
                re-flowed
            to fit
        the width
    of the
window.

Separate paragraphs from one another with blank lines.

Inside paragraphs you can write **bold text** by surrounding words with two asterisks, `**`.
_Italicized text_ is surrounded by single underlines `_`.
~~Struck through text~~ is surrounded by double tildes `~~`.
A `code span` is created by surrounding text with a back-tick `` ` ``
(**_Hint_**: back-tick shares the same key as `~`).
```



## Pre-formatted Code Blocks

Unlike paragraphs, pre-formatted code blocks preserve your indentation and spacing *exactly*.

The following is intentionally redundant; first you will see an example of a code block followed by a code block that shows how I made the code block.

```
Pre-formatted
    blocks
        of
            text
        (i.e. code blocks)
            Are made by indenting a block of text by four spaces,
                or fencing a block of text with triple back-ticks ```
            or with triple tildes ~~~

A fence is a line that starts with and contains only 3 of the same character:

~~~
For example,
I'm surrounded by a fence of triple tildes
~~~
```


    ```
    Pre-formatted
        blocks
            of
                text
            (i.e. code blocks)
                Are made by indenting a block of text by four spaces,
                    or fencing a block of text with triple back-ticks ```
                or with triple tildes ~~~

    A fence is a line that starts with and contains only 3 of the same character:

    ~~~
    For example,
    I'm surrounded by a fence of triple tildes
    ~~~
    ```

Here is another example:

    Another way to form a code block in Markdown
    is to indent a paragraph by four spaces.


```
    Another way to form a code block in Markdown
    is to indent a paragraph by four spaces.
```


If GitLab knows about your programming language, it can present code with
**syntax highlighting**.  Write the name of the programming language
immediately after the opening triple-backquote, like this: `` ```python ``.

```python
# you can even
def code_blocks(with, programming, language, syntax, highlighting)
    """
    by writing the name of the programming language
    after the first triple-character fence
    """
    if this == pretty_cool:
        return True
```

    ```python
    # you can even
    def code_blocks(with, programming, language, syntax, highlighting)
        """
        by writing the name of the programming language
        after the first triple-character fence
        """
        if this == pretty_cool:
            return True
    ```



## Tables

| Tables | with     | columns |
|--------|----------|---------|
| can    | be       | made    |
| with   | pipes,   | spaces, |
| and    | a        | lot     |
| of     | patience | !       |
| The    | important| thing   |
| is     | that     | the     |
| line   | following| the     |
| header | consists | of      |
| dashes


```
| Tables | with     | columns |
|--------|----------|---------|
| can    | be       | made    |
| with   | pipes,   | spaces, |
| and    | a        | lot     |
| of     | patience | !       |
| The    | important| thing   |
| is     | that     | the     |
| line   | following| the     |
| header | consists | of      |
| dashes
```



## Lists

*   Bulleted
*   lists
    *   may contain
    *   indented
    *   sub-lists
-   Items are prefixed with such characters as:
    *   `*` asterisks
    +   `+` plus Signs
    -   `-` minus Signs

```
*   Bulleted
*   lists
    *   may contain
    *   indented
    *   sub-lists
-   Items are prefixed with such characters as:
    *   `*` asterisks
    +   `+` plus Signs
    -   `-` minus Signs
```


0.  Ordered
0.  lists
    *   may also contain
    *   indented
    *   sub-lists
    *   bulleted or ordered are both okay
0.  List items begin with...
    1.  ...digits, followed by a period `.`
    2.  It doesn't matter which digit prefixes items at the top-level of the list
    3.  But numbered sub-lists must begin at `1.`


```
0.  Ordered
0.  lists
    *   may also contain
    *   indented
    *   sub-lists
    *   bulleted or ordered are both okay
0.  List items begin with...
    1.  ...digits, followed by a period `.`
    2.  It doesn't matter which digit prefixes items at the top-level of the list
    3.  But numbered sub-lists must begin at `1.`
```



## Task Lists

*   [X] A bulleted or numbered list becomes a **task list** when the first item after the list marker is a pair of *square brackets* containing a space ` `, `x` or tilde `~`
    *   [ ] *Incomplete* tasks are an empty pair of square brackets with a space in between `[ ]`
    *   [X] *Completed* tasks are a pair of square brackets with an `X` in between `[X]`
    *   [~] A cancelled or *inapplicable* task is a pair of square brackets surrounding a tilde `[~]`
*   [ ] Task lists appear in the Software Development Plan to help you keep track of important tasks
*   [X] These checkboxes are a *special feature* in GitLab
    *   [ ] Not every Markdown system recognizes task lists

```
*   [X] A bulleted or numbered list becomes a **task list** when the first item after the list marker is a pair of *square brackets* containing a space ` `, `x` or tilde `~`
    *   [ ] *Incomplete* tasks are an empty pair of square brackets with a space in between `[ ]`
    *   [X] *Completed* tasks are a pair of square brackets with an `X` in between `[X]`
    *   [~] A cancelled or *inapplicable* task is a pair of square brackets surrounding a tilde `[~]`
*   [ ] Task lists appear in the Software Development Plan to help you keep track of important tasks
*   [X] These checkboxes are a *special feature* in GitLab
    *   [ ] Not every Markdown system recognizes task lists
```



## Hyperlinks

[Hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_hyperlinks) are an important feature of the [World Wide Web](https://developer.mozilla.org/en-US/docs/Glossary/World_Wide_Web).  These are written in two parts:

0.  Surround the text of the link with square brackets `[]`
1.  Surround the address in parentheses `()`
2.  All together, it looks like `[this](http://example.com/)`...
3.  ...And works like [this](http://example.com/)

```
[Hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_hyperlinks) are an important feature of the [World Wide Web](https://developer.mozilla.org/en-US/docs/Glossary/World_Wide_Web).  These are written in two parts:

0.  Surround the text of the link with square brackets `[]`
1.  Surround the address in parentheses `()`
2.  All together, it looks like `[this](http://example.com/)`...
3.  ...And works like [this](http://example.com/)
```


## Images

Images are like Hyperlinks that start with a `!`.

1.  Within the square brackets `![]` write the alt-text for the image
    *   The *alt-text* is shown when the image cannot be loaded or displayed
2.  Write the address of the image surrounded by parentheses `()`
    *   **Optional** within the parentheses you may also write a *title* for the image as a quoted string
    *   The *title* is the text shown when your mouse hovers over the image
3.  All together, it looks like this `![Meme: a man nervously deliberating which button to push](./assets/two-buttons.jpg "it's the one on the right...")`
4.  ...And works like this:
    *   ![Meme: a man nervously deliberating which button to push](./assets/two-buttons.jpg "it's the one on the right...")

```
Images are like Hyperlinks that start with a `!`.

1.  Within the square brackets `![]` write the alt-text for the image
    *   The *alt-text* is shown when the image cannot be loaded or displayed
2.  Write the address of the image surrounded by parentheses `()`
    *   **Optional** within the parentheses you may also write a *title* for the image as a quoted string
    *   The *title* is the text shown when your mouse hovers over the image
3.  All together, it looks like this `![Meme: a man nervously deliberating which button to push](./assets/two-buttons.jpg "it's the one on the right...")`
4.  ...And works like this:
    *   ![Meme: a man nervously deliberating which button to push](./assets/two-buttons.jpg "it's the one on the right...")
```




## Markdown Hints

*   Paragraphs must be separated from each other with *blank* lines
    *   If your paragraphs run together, add extra blank lines in between
*   **Do not** write Markdown directly in GitLab's Web IDE.
    *   Although GitLab has a preview feature, it creates problems when syncing your code between the server and your computer.
    *   PyCharm and VS Code can display a live preview of Markdown files.
        *   If you want to see what your Markdown files will look like as you write, this is the best way to go.
        *   Be aware that some of GitLab's special Markdown extensions will not look the same in your IDE's previewer



## More resources

*   [The Markdown Guide](https://www.markdownguide.org/) a free and open-source reference guide
*   [GitLab Flavored Markdown](https://gitlab.cs.usu.edu/help/user/markdown.md) describes how Markdown works on this site
*   [Markdown on John Gruber's Blog](https://daringfireball.net/projects/markdown/) straight from the horse's mouth


*Updated Wed Sep 18, 2024*
