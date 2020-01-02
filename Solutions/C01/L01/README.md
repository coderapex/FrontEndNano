# C01 - L01 - HTML

- [C01 - L01 - HTML](#c01---l01---html)
  - [01. Course Introduction](#01-course-introduction)
  - [02. Intro to HTML](#02-intro-to-html)
  - [03. Text Editors](#03-text-editors)
  - [04. Exercise: Creating an HTML File](#04-exercise-creating-an-html-file)
  - [05. Text Elements I](#05-text-elements-i)
  - [06. Text Elements II](#06-text-elements-ii)
  - [07. HTML Lists](#07-html-lists)
      - [Unordered Lists](#unordered-lists)
      - [Ordered Lists](#ordered-lists)
      - [Description Lists](#description-lists)
  - [08. Attributes](#08-attributes)
      - [Images](#images)
        - [Links](#links)
      - [Comments](#comments)
      - [Self-Closing Elements](#self-closing-elements)
  - [09. The DOM](#09-the-dom)
  - [10. Exercise: Creating an HTML Template](#10-exercise-creating-an-html-template)
  - [11. Forms](#11-forms)
  - [12. Exercise: Debugging HTML](#12-exercise-debugging-html)
  - [13. Recap](#13-recap)

**Note**: A substantial amount of content in this repo is copy-pasted from the Udacity program. I am maintaining this repo to be able to reference learning material from the course after access has been revoked on program completion.

---

## 01. Course Introduction

An introduction to the course.

## 02. Intro to HTML

Provides an overview of what HTML is and how it works along with CSS and Javascript to create interactive web pages.

## 03. Text Editors

### Notes <!-- omit in toc -->

- HTML documents can be opened in two ways:
  - By browsers where they process the contents and render the output.
  - By text editors where they show the contents as plain text.

### Activity <!-- omit in toc -->

1. Download and install a text editor or IDE.
2. Write `<p>Hello World!</p>` in a text editor.

## 04. Exercise: Creating an HTML File

### Notes <!-- omit in toc -->

- Read instructions in the `Instructions.md` file and follow accordingly.

### Activity <!-- omit in toc -->

- Create an HTML File `index.html` and display `<p>Hello World</p>`.

[**Solution**](/04/)

---

## 05. Text Elements I

### Notes <!-- omit in toc -->

#### General Text Element Structures <!-- omit in toc -->

Syntax : `<p class="class-name">Text here</p>`

1. **The opening tag** is the first HTML tag used to start an element.
2. **The content** is the info contained between the opening and closing tags. Only this content inside the opening and closing body tags is displayed to the screen.
3. **The closing tag** is the second tag used to define the end of a single element. Closings tags have a forward slash / inside of them, always after the left angle bracket.
4. (Optional) **The attribute** name and value.

#### Block and Inline Elements <!-- omit in toc -->

##### Block Elements <!-- omit in toc -->

Block elements are meant to structure the main parts of your page, by dividing your content in coherent blocks.

Block elements are:

- paragraphs `<p>`
- lists:
  - unordered (with bullet points) `<ul>`, or
  - ordered - lists (with numbers) `<ol>`
- headings: from 1st level `<h1>` to 6th level headings - `<h6>`
- articles `<article>`
- sections `<section>`
- long quotes `<blockquote>`

##### Inline Elements <!-- omit in toc -->

Inline elements are meant to differentiate part of a text, to give it a particular function or meaning. Inline elements usually comprise a single or few words.

Inline elements are:

- links `<a>`
- emphasized words `<em>`
- important words `<strong>`

### Activity <!-- omit in toc -->

There is no proposed activity for this lesson per se. Although for reference I have made an HTML which uses the block and inline elements discussed above.

[**Solution**](/05/)

---

## 06. Text Elements II

### Notes <!-- omit in toc -->

#### Headings <!-- omit in toc -->

Headings are the primary way to outline the content of your webpage. They define the outline of your web page as both humans and search engines see it, which makes selecting relevant headings essential for a high-quality web page.

The code sample used to illustrate this is :

```html
<h1>Observable Universe</h1>
<h2>Milky Way Galaxy</h2>
<h3>Earth</h3>
<h4>USA</h4>
<h5>Norfolk, VA</h5>
<h6>Main Street</h6>
```

##### Accessibility by headers <!-- omit in toc -->

For people who are blind or visually impaired, screen reading software is used to parse through text on a web page. A common technique these folks will use to navigate the page is to jump from heading to heading to determine the overall content of the page more easily.

If you did skip headings and went from `<h1>` to `<h3>`, you may cause confusion since the user has to deal with a missing heading.

#### Paragraphs <!-- omit in toc -->

Paragraphs act as the default block-level element of HTML documents.

The code sample used to illustrate this is :

```html
<p>
  The sweet-faced and loving Labrador Retriever is actually one of the most
  popular dog breeds.
</p>
<p>
  Labs are extremely friendly with an easygoing and high-spirited personality
  which is great for bonding with the whole family.
</p>
```

#### Span <!-- omit in toc -->

The HTML `<span>` element is like a generic wrapper that is used to group text, mostly for styling purposes.

The code sample to illustrate this is :

```html
<style>
  p {
    color: black;
  }
  .red {
    color: red;
  }
</style>
<p>
  This sentence needs some <span class="”red”">visual emphasis</span> to really
  bring home the point.
</p>
```

#### Blockquote <!-- omit in toc -->

Blockquotes are used to identify a citation.

```html
<blockquote cite="https://www.wikiwand.com/en/Scooby-Doo_(character)">
  <p>Ruh-roh--RAGGY!!!</p>
  <footer>—Scooby Doo, <cite>Mystery Incorporated</cite></footer>
</blockquote>
```

#### Line Breaks <!-- omit in toc -->

In order to modify the default spacing and line breaking of HTML we use the `<br />` element.

### Activity <!-- omit in toc -->

Internal quiz.

## 07. HTML Lists

### Notes <!-- omit in toc -->

HTML Lists are of three types:

1. Unordered Lists
2. Ordered Lists
3. Description Lists

#### Unordered Lists

The syntax for unordered lists is :

```html
<ul>
  <li>This is</li>
  <li>an unordered</li>
  <li>list.</li>
</ul>
```

`ul` - Unordered list tag
`li` - List item tag

#### Ordered Lists

The syntax for ordered lists is very similar to that or unordered list :

```html
<ol>
  <li>This is</li>
  <li>an unordered</li>
  <li>list.</li>
</ol>
```

`ol` - Ordered list tag
`li` - List item tag

**OUTPUT**:

<ol>
  <li>This is</li>
  <li>an unordered</li>
  <li>list.</li>
</ol>

#### Description Lists

Description lists are lists with key value pairs. The syntax for description lists is :

```html
<p>Making Power-Puff Girls</p>

<dl>
  <dt>Sugar</dt>
  <dd>A large jar of white and brown sugar.</dd>

  <dt>Spice</dt>
  <dd>ALL of them.</dd>

  <dt>Everything Nice</dt>
  <dd>Chocolates, candies and more.</dd>
</dl>
```

`dl` - Description list
`dt` - Description title
`dd` - Description details

**OUTPUT**:

<p>Making Power-Puff Girls</p>

<dl>
  <dt>Sugar</dt>
  <dd>A large jar of white and brown sugar.</dd>

  <dt>Spice</dt>
  <dd>ALL of them.</dd>

  <dt>Everything Nice</dt>
  <dd>Chocolates, candies and more. </dd>
</dl>

### Activity <!-- omit in toc -->

Created a HTML File with all three types of lists.

[**Solution**](/07/)

## 08. Attributes

### Notes <!-- omit in toc -->

 Attributes provide additional information about an element, and are always specified in the start tag. Attributes usually come in name/value pairs like `name="value"`.

#### Images

- The “source” (URL or file location) from where an image is taken through the `src` attribute
- The image’s alternative text (often a description for those with accessibility needs) is provided through the `alt` attribute
- The image size can be adjusted through the `width` and `height` attributes
- Images are self-closing - you add a slash at the end, instead of another `</img>` tag as we have seen before

##### SYNTAX <!-- omit in toc -->

```html
<img
  src="image url"
  alt="description of image"
  width="480"
  height="320"
/>
```

##### Links

n HTML, links are inline elements written with the <a> tag. The href attribute (hypertext reference) is used to define the destination of the link.

There are 3 types of destinations you can define:

- anchor targets, to navigate within the same page
- relative URLs, usually to navigate within the same website
- absolute URLs, usually to navigate to another website

Additional attributes besides `a` and `href` that can be used are:

- `rel` attribute to specify the relationship between the current and linked document
  - example: `rel="noopener"` prevents a link from being able to access the `window.opener` property and ensures it runs in a separate process with the `noopener` rel value.
- `target` attribute - specify where to open the linked document
  - example: `_blank` requests the browser to open the link in a new window instead of the same one with where the link is displayed

##### SYNTAX <!-- omit in toc -->

```html
<a href="www.coderapex.com" rel="noopener" target="_blank" >Visit CoderApex.com</a>
```

<a href="www.coderapex.com" rel="noopener" target="_blank" >Visit CoderApex.com</a>

#### Comments

Comments will be ignored by the browser. They are to any person who will be reading the source code in the future. That could be any developer on the team or outside the organization, or even yourself in the future.

A comment starts with `<!--` and ends with `-->`.

##### SYNTAX <!-- omit in toc -->

```html
<!-- Place comment here -->
```

#### Self-Closing Elements

Certain HTML Elements like `<br />`, `<hr>`, `<input>`, etc. are self closing and will not have any closing tags.

As they do not have any closing tags, they cannot contain any content inside them. They generally have attributes that help provide more information.

##### SYNTAX <!-- omit in toc -->

```html
<!-- line-break -->
<br />
<!-- image -->
<img src="#" alt="Img description" />
<!-- text input -->
<input type="text" />
```

## 09. The DOM

### Notes <!-- omit in toc -->

Notes here

### Activity <!-- omit in toc -->

Activity here

**Solution**

## 10. Exercise: Creating an HTML Template

### Notes <!-- omit in toc -->

Notes here

### Activity <!-- omit in toc -->

Activity here

**Solution**

## 11. Forms

### Notes <!-- omit in toc -->

Notes here

### Activity <!-- omit in toc -->

Activity here

**Solution**

## 12. Exercise: Debugging HTML

### Notes <!-- omit in toc -->

Notes here

### Activity <!-- omit in toc -->

Activity here

**Solution**

## 13. Recap

### Notes <!-- omit in toc -->

Notes here

### Activity <!-- omit in toc -->

Activity here

**Solution**
