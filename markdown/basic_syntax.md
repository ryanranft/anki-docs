# Markdown Guide

## Basic Syntax

### Headings

To create a heading, add one to six `#` symbols before your heading text. The number of `#` you use will determine the size of the heading.

#### Alternate Heading Syntax

Below text you want to turn into a heading, add a line of `=` or `-` characters. The `==` character will create a level heading, while the `--` character will create a level 2 heading.

#### Heading Best Practices

Add a space between the `#` and your heading text. For example, `# Heading 1` is correct, while `#Heading 1` is incorrect.

Add a blank line before and after your heading. This will help with readability and ensure that your headings are properly formatted.

### Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text. For example:

```
This is the first paragraph.

This is the second paragraph.
```

#### Paragraph Best Practices

A blank line is not required if you write a paragraph in HTML, but it is recommended for readability.

<p>There is no spacing between this html paragraph and the next one.</p>
<p>It is best practices to add a blank line between a blank line when writing text paragraphs with html syntax, however is is easier to read when there is a space.</p>

Do not put tabs or spaces in front of your paragraph text.

Keep lines left-aligned

### Line Breaks

The line breaks created by adding two spaces at the end of a sentence on the same line. For example:

```
This is the first sentence of a before adding two spaces after the period.  This is the second line, and second sentence of the same paragraph.
````
Hi,<br>there are several line breaks in this text. <br>Line breaks are created by adding the &lt;br&gt; tag.

Two or more spaces are commonly referred to as "Trailing whitespace". Trailing whitespace is not recommended, as it can cause formatting issues in some cases. It is best to use the `<br>` tag for line breaks instead.

While writing this markdown document, I have noticed that the line breaks are not being rendered correctly in some cases. This is likely due to the fact that the markdown parser is not recognizing the trailing whitespace as a line break. To avoid this issue, it is best to use the `<br>` tag for line breaks instead of relying on trailing whitespace.  I disabled the trailing whitespace in my text in the settings via files.trimTrailingWhitespace.  The trailing whitespace is still present in the text, but it is not being rendered as a line break.  I will continue to use the `<br>` tag for line breaks in this document to ensure that they are rendered correctly. I also enabed white space rendering in my settings via files.renderWhitespace.  This will allow me to see the trailing whitespace in my text, and ensure that it is not causing any formatting issues.  I will continue to use the `<br>` tag for line breaks in this document to ensure that they are rendered correctly. Further work needs to be done to determine why the trailing whitespace is not being rendered as a line break in some cases, and to find a solution to this issue.

### Emphasis

#### Bold

To create bold text, add two asterisks `**` or underscores `__` before and after the text you want to make bold. For example:

**This text has two asterisks before and after the sentence.**

__This text has two underscores before and after the sentence.__

**T**he first and last letters of this sentence are bolded, while the rest of the sentence is no**t**.

##### Bold Best Practices

Markdown applications don't agree underscores on how to handle underscores in the middle of a word. For compatibility, it is best to use asterisks for bolding text in the middle of a word.

Example: `**t**his is a test` will render as **t**his is a test, while `__t__his is a test` will render as __t__his is a test.

#### Italic

To create italic text, add one asterisk `*` or underscore `_` before and after the text you want to make italic. For example:

*This text has one asterisk before and after the sentence.*

_This text has one underscore before and after the sentence._

*T*he first and last letters of this sentence are italicized, while the rest of the sentence is no*t*.

##### Italic Best Practices

Markdown applications don't agree on how to handle underscores in the middle of a word. For compatibility, it is best to use asterisks for italicizing text in the middle of a word.

Example: `*t*his is a test` will render as *t*his is a test, while `_t_his is a test` will render as _t_his is a test.

#### Bold and Italic

To create bold and italic text, add three asterisks `***` or underscores `___` before and after the text you want to make bold and italic. For example:

***This text has three asterisks before and after the sentence.***

___This text has three underscores before and after the sentence.___

***T***he first and last letters of this sentence are bolded and italicized, while the rest of the sentence is no***t***.

Any combination of asterisks and underscores can be used to create bold and italic text. For example, `**_This text has two asterisks and one underscore before and after the sentence._**` will render as **_This text has two asterisks and one underscore before and after the sentence._**.

##### Bold and Italic Best Practices

Markdown applications don't agree on how to handle underscores in the middle of a word. For compatibility, it is best to use asterisks for bolding and italicizing text in the middle of a word.

Example: `***this is a test of best practices***` will render as ***this is a test of best practices***, while `__*t*__his is a test` will render as __*t*__his is a test.

### Blockquotes

To create a blockquote, add a `>` in front of a paragraph. For example:

> Dorothy followed the yellow brick road to the Emerald City, where she met the Wizard of Oz. The Wizard granted her wish to return home to Kansas, and she lived happily ever after.

#### Blockquotes with Multiple Paragraphs

Blockquotes can contain multiple paragraphs. To create a blockquote with multiple paragraphs, add a `>` on the blank lines between the paragraphs. For example:

```
>Dorothy followed the yellow brick road to the Emerald City, where she met the Wizard of Oz.
>
>The Wizard granted her wish to return home to Kansas, and she lived happily ever after.
```

>Dorothy followed the yellow brick road to the Emerald City, where she met the Wizard of Oz.
>
>The Wizard granted her wish to return home to Kansas, and she lived happily ever after.

#### Nested Blockquotes

Blockquotes can be nested. Add a '>>' in front of a line to create a nested blockquote. For example:

```
> Dorothy followed the yellow brick road to the Emerald City, where she met the Wizard of Oz.
>
>> The Wizard granted her wish to return home to Kansas, and she lived happily ever after.
```

The rendered output looks like this:

> Dorothy followed the yellow brick road to the Emerald City, where she met the Wizard of Oz.
>
>> The Wizard granted her wish to return home to Kansas, and she lived happily ever after.

#### Blockquotes with Other Elements

Blockquotes can contain other elements. Not all elements can be used -- experiment to see which ones work.

Example:

```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everything* is going according to **plan**.
```

The rendered output looks like this:

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everything* is going according to **plan**.

#### Blockquote Best Practices

For compaltibility, put blank lines before and after blockquotes.

```
Try to put a blank line before...

> This is a blockquote.

... and after a blockquote.
```
Try to put a blank line before...

> This is a blockquote.

... and after a blockquote.

### Lists

Items can be organized into ordered and unordered lists.

#### Ordered Lists

To create an ordered list, add a number followed by a period and a space before each item. The numbers don't have to be in numerical order, but the list list should start with the the number 1.

For example:

```
1. First item
2. Second item
3. Third item
```
Rendered output looks like this:
1. First item
2. Second item
3. Third item

```
1. First item
8. Second item
3. Third item
5. Fourth item
```
Rendered output looks like this:
1. First item
8. Second item
3. Third item
5. Fourth item

```
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item
```

Rendered output looks like this:
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

##### Ordered List Best Practices

Some lightweight markup languages allow the use of parenthesis instead of periods for ordered lists. For example, `1)` instead of `1.`. However, this is not supported in all markdown applications, so it is best to use periods for compatibility.

#### Unordered Lists

To create an unordered list, add a `-`, `+`, or `*` followed by a space before each item. For example:

```
- First item
- Second item
- Third item
- Fourth item
```
Rendered output looks like this:
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

##### Starting Unordered List Items With Numbers

To start an unordered list item with a number, add a backslash `\` to escape the number.
For example:

```
- 1968\. A great year!
- I think 1969 was second best.
```
- 1968\. A great year!
- I think 1969 was second best.

###### Unordered List Best Practices

Different delimitters can be used for unordered lists, but it is best to use the same delimiter for all items in a list. For example, if you start a list with `-`, use `-` for all items in that list. This will ensure that your list is properly formatted and easy to read.

#### Adding Elements in Lists

Indentation with the tab key is equal to four spaces.

##### Paragraphs

```
* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.
    
* And here's the third list item.
```

The rendered output looks like this:

* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.
    
* And here's the third list item.

##### Blockquotes

```
* This is the first list item.
* Here's the second list item.

    > A blockquote would look great below the second list

* And here's the third list item.
```

The rendered output looks like this:

* This is the first list item.
* Here's the second list item.

    > A blockquote would look great below the second list

* And here's the third list item.

##### Code Blocks

Code blocks are normally indented four spaces or one tab. When code blocks are inside a list, indent them eight spaces or two tabs.

Example:

```
1. Open the file
2. Find the following code block on line 21:

        <html>
            <head>
                <title>Test</title>
            </head>

3. Update the title to match the name of your website.
```

The rendered output looks like this:

1. Open the file
2. Find the following code block on line 21:

        <html>
            <head>
                <title>Test</title>
            </head>

3. Update the title to match the name of your website.

##### Images

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

![Tux, the Linux mascot](https://www.markdownguide.org/assets/images/generated/assets/images/tux-1080.png)

3. Close the file.

##### Lists

Nesting an unordered list inside an ordered list. An ordered list can also be nested inside of an unordered list.

```
1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item
```

The rendered output looks like this:

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

### Code

To denote a word or phrase as code, enclose it in backticks (`).

At the command prompt, type `nano`. 

#### Escaping Backticks

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks(``).

```
``Use `code` in your Markdown file.``
```

The rendered output looks like:

``Use `code` in your Markdown file.``

#### Code Blocks

Code blocks are created by indenting every line by at least four spaces or one tab.

```
    <html>
        <head>
        </head>
    <html>
```

The rendered output looks like this:

    <html>
        <head>
        </head>
    <html>

To create code blcks without indenting lines, use fenced code blocks

### Horizontal Rules

To creaete a horizontal rule, use three or more asterisks (***), dashes (---), or underscores(___) on a line by themselves.

```
***
---
__________________
```

The rendered output of all three looks identical:

***
---
__________________

### Horizontal Rule Best Practices

Blank lines before and after horizontal rules are best practices.

Try to put a blank line before...

---

...and after a horizontal rule

Without blank lines between text and horizontal rules, this would be a heading.
---
Do not do this

### Links

To create a link, enclose the link text in brackets (e.g., [Brave Browser]) and then follow it immediately with the URL in parentheses (e.g., (https://brave.com)).

    My favorite search engine is [Brave browser](https://brave.com) "The best search engine for privacy".

The rendered output looks like this:

My favorite search engine is [Brave browser](https://brave.com "The best search engine for privacy").

> [!NOTE]
> To link to an element on the same page, see [linking to heading IDs](#heading-ids). Learn how to link heading ID's and how to open a new tab or window to see the section on [link targets](#link-targets).

Learn how to link heading ID's and how to open a new tab or window to see the section on link targets.

#### Adding Titles

It is optional to add a title to a link. The title of the link will appear as a tooltip when the user hovers over the link. To add a title, enclose it in quotation marks after the URL.

```
My favorite search engine is [Brave Browser](https://brave.com "The best search engine for privacy").
```

The rendered output looks like this:

My favorite search engine is [Brave Browser](https://brave.com "The best search engine for privacy").

#### URLs and Email Addresses

To quickly turn a URL or email address into a link, enclose it in angle brackets.

<https://www.markdownguide.org>
<fake@example.com>

#### Formatting Links

To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.

```
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
```

The rendered output looks like this:

