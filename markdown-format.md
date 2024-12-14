# Formatting Github Markdown

## Table of Content
- [Headings](#headings)
- [Text Styles](#text-styles)
- [Hyperlinks](#hyperlinks)
- [Lists](#lists)
  - [Unordered List](#unordered-list)
  - [Ordered List](#ordered-list)
  - [Mixed List](#mixed-list)
  - [Task Lists](#task-lists)
- [Block Quotes](#block-quotes)
  - [Alerts](#alerts)
- [Block Codes](#block-codes)
- [Tables](#tables)

## Headings
```md
# First-level heading
## Second-level heading
### Third-level heading
#### Fourth-level heading
##### Fifth-level heading
###### Sixth-level heading
```
> [!NOTE]
> - The font of forth-level heading and above is smaller than normal font.
> - The sixth-level heading turns the text into grey.
> - Declaring two or more headings will create <ins>fragment identifier (#)</ins> that can be use to jump to specific heading using [hyperlinks](#hyperlinks)

## Text Styles
Style|Syntax|Shortcut
---|:---:|:---:
**Bold**|`** **` or `__ __`|`Ctrl` + `B`
_Italic_|`* *` or `_ _`|`Ctrl` + `I`
~~Strikethrough~~|`~~ ~~`|None
<ins>Underline</ins>|`<ins> </ins>`|None
<sup>Superscript</sup>|`<sup> </sup>`|None
<sub>Subscript</sub>|`<sub> </sub>`|None
> [!NOTE]
> The style of Strikethrough and Underline aren't displaying their Preview while editing file. They'll look normal after commiting the change.

## Hyperlinks
```md
# Syntax: [title](href)

[URL](https://github.com/) <!--- Link to https://github.com/ -->
[Anchor](#table-of-content) <!--- Jump to Table of Content in this file -->
[Path](./markdown-format.md) <!--- Link to ./markdown-format.md in this repository -->
```
**Output:**
> [URL](https://github.com/)
> [Anchor](#table-of-content)
> [Path](./markdown-format.md)

## Images
```md
# Syntax: ![alt](source-url)

![Github Banner](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRd6e6lvbBEi8ypefp5JrKZregYbTNk17Bdhg&s)
```
**Output:**  
> ![Github Banner](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRd6e6lvbBEi8ypefp5JrKZregYbTNk17Bdhg&s)

## Lists
### Unordered List
```md
# Prefix: * - +

* Content 1
- Content 2
  - Content 2.1
    - Content 2.1.1
  + Content 2.2
* Content 3
```
**Output:**
> * Content 1
> - Content 2
>   - Content 2.1
>     - Content 2.1.1
>   + Content 2.2
> * Content 3

### Ordered List
```md
# Prefix: number

1. Content 1
3. Content 2
   1. Content 2.1
   4. Content 2.2
      1. Content 2.2.1
5. Content 3
```
**Output:**
> 1. Content 1
> 3. Content 2
>    1. Content 2.1
>    4. Content 2.2
>       1. Content 2.2.1
> 5. Content 3

> [!NOTE]
> Order doesn't matter, but first child must be "1"

### Mixed List
```md
- Content 1
  1. Content 1.1
  2. Content 1.2
- Content 2
- Content 3
  - Content 3.1
    1. Content 3.1.1
    2. Content 3.1.2
```
**Output:**
> - Content 1
>   1. Content 1.1
>   2. Content 1.2
> - Content 2
> - Content 3
>   - Content 3.1
>     1. Content 3.1.1
>     2. Content 3.1.2

### Task Lists
```md
- [x] Make functional code
- [ ] Make information clear
```
**Output:**
> - [x] Make functional code
> - [ ] Make information clear

## Block Quotes
```md
# Prefix: >

> This is a block quote
> > Double block quote !!!
```
**Output:**
> > This is a block quote
> > > Double block quote !!!

### Alerts
```md
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
```
**Output:**
> ![Alerts](https://docs.github.com/assets/cb-24696/mw-1440/images/help/writing/alerts-rendered.webp)

## Block Codes
````md
This is `an inline code`

```
A code block
```

```py
print("A code block with format highlight")
```
````
**Output:**
> This is `an inline code`
> 
> ```
> A code block
> ```
> 
> ```py
> print("A code block with format highlight")
> ```

## Tables
```
Header 1|Header 2|Header 3
:-------|:------:|-------:
Left    |Center  |Right
A       |B       |C
1       |2       |3
```
> Header 1|Header 2|Header 3
> :---|:---:|---:
> Left|Center|Right
> A|B|C
> 1|2|3
