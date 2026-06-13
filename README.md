# HTML

learn HTML

=======================START HTML=============================================

- inside html tags, -> head and body
<head> content is not displayed on the screen
<body> content is.

- use w3c validator to check and validate html files.
- provide a language inside html tag. eg:-> <html lang="en>
- then add character set between <head></head> tags with a <meta> tag
  eg:-> <head>
  <meta charset="UTF-8">
  </head>

- add <!DOCTYPE html> tag at the top of the file

Do these steps to setup html file so there are no errors after validating

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>TITLE TEXT</title>
    </head>
    <body>
        <h1>HEADER TEXT</h1>
        <p>PARAGRAPH TEXT</p>
    </body>
</html>

# The text should look like this.

    MORE META TAGS

<meta name="author" content="author name">
<meta name="description" content="description content">

    LINK TAGS

<link rel="" href=""> 
rel - relationship between the linking file and HTML page
href - hypertext reference (link to the location of the file)

# rel : icon, stylesheet

- have only one H1 in html.
- Headers have some semantic meanings.

================================================================================
-block level elements

- <h> tags, <br>, <hr>, <p> ..etc are block level elements. They take up a whole line and at the end it moves to a new line.
- unless they are formatted with css they take the whole device width.
- if I a paragraph inside a <p> tag it will create a new line where the paragraph on the inside starts.

-inline elements

- <em>(emphasise), <strong>, <abbr>(abbreviations)

-html entities

- start with & end with ;
  &nbsp - indent
  &lt - lower than sign
  &gt - greater than sign
  &copy - copywrite sign

==================================================================================
LISTS
-ordered list (Numbered list) <ol></ol>
-unordered list (Point list) <ul></ul>
-list items (Content inside Ols and Uls.) <li></li>

-description list () <dl></dl>
-this list type has two elements inside:
*Description Term <dt></dt>
*Description Detail <dd></dd>

==================================================================================
LINKS
-Use an anchor tag <a></a>
-Relative reference, Absolute reference, Internal reference.
(link to lanugages-> absolute, link to about page-> relative)
_(<section> semantic tag to divide the page into seperate sections)
_(link the section using a <a> tag to the section with its id)
_(use '#'infornt of the section id when refering to a section eg:- #section-one)
_('#' points to the top of the page)

use download attribute to download a file with a link
<a href="favicon.png" download>DOWNLOAD</a> (this link will download the file. but the file has to be in the project folder)
<a href="mailto:random@gmail.com">EMAIL</a> (use mailto: inside the href)
<a href="tel:0112729729">PHONE</a> (use tel: inside the href)
<a href="https://website.com" target="_blank">RANDOM SITE</a> (open the link in a new tab with target="\_blank")

<nav> - check semantics

===================================================================================
IMAGES

-have a seperate file to store static images for the website
-use <img> tag

- src - give the location of the image
- alt - alternate text incase the image fails
- title - this text will show when the cursor is on the image
- width/height - set the size of the image
- loading - set to "lazy" if the image is below the fold.

<figure> is a container to wrap around the image perfectly by grouping the image and the caption
use <figcaption></figcaption> inside figure tags to write a caption.
make sure <figcaption> is the first or the last inside the figure element

\*\*\*\*although, figure element is not only for images.

using figure elements gives a little indentation to the images and push them to the center.
image 3 is little indented, less than image 2.

the second image is more towards to the center because its in a list element. so the figure gives indentation to the already indented list element.

can use <code> element to insert a code inside a figure

---

==image sites==
placehold.co
unsplash.com
pexels.com
gratisography.com
pixabay.com

irfanview

=====================================================================================
SEMANTICS

using semantic elements let us nvaigate through different sections and pages of the website.

heirarchy -> 1 <h1> hearders

<nav> - used to define a section of a page that contains navigation links (either to other pages or different parts within the same page)
  eg:-
      <nav>
          <ul>
              <li><a href="#html-section">LEARN HTML</a></li>
              <li><a href="#vacation-section">VACATION </a></li>
          </ul>
      </nav>

<hr> =is also a semantic element meaning there is a topic change.
<header> = element is a structural semantic tag used to group introductory content,        navigational links, or branding information. can use the <header> inside <article> or       <section> tags to group title information.
<main> = only one main element for a page.
<footer> = can have multiple in a page.
  No nesting headers: You cannot put a <header> inside another <header>.
  No footers allowed: A <header> cannot contain a <footer> element.
  It does not mean <head>: This is the most frequent beginner mix-up.
      <head> is a invisible container for metadata, CSS links, and page titles that stays hidden from the user.
      <header> is visible layout content that users see on the page.
  Headings vs. Headers: An <h1> tag is just a text heading. A <header> is a container box that can hold an <h1>, subtitles, images, and other wrapper elements.

semantic tags give meaning to the section of the page and helps screen readers and other functions.

<article> = The <article> element is a structural semantic tag used to wrap a piece of content that is completely self-contained, independent, and reusable.

<article> vs <section>
<article> is independent. It is a whole entity on its own (e.g., a whole book, a whole newspaper article).

<section> is dependent. It is a thematic grouping of content, usually used to split up a single larger document into chapters or chunks (e.g., a "Contact Us" section, or "Chapter 1" of an article).

<aside> = is a structural semantic tag used for content that is tangentially related to the main content around it, but could be separate.

<details> = is a built-in semantic HTML tag used to create a native accordion widget—a collapsible dropdown section that the user can expand or hide by clicking.

<summary> = This acts as the clickable heading or label. The browser automatically places a small disclosure triangle (arrow) next to it.

<mark> = highlights the text within

<time datetime=""> = when we use time or date
  eg:- <time datetime="06:00">6 AM</time> (06:00 does not show up but its helpful to assistive technology and the browser)
  eg:-<time datetime="PT3H">3 hours</time> (3 Hours)

=====================================================================================
TABLES

<table> -  Table stores tabular data  (arrange items in the table to columns and rows)
<tr> - Table Row (Define a row and th or td in the row act as columns)
<td> - Table Details (Add content in the row as columns)
<th> - Table Headings (Add heading to the table inside a row) (by default it is centered, bold)
<caption> - To add a caption to the table. (Will create a row on top of the table without breaking into columns)
<thead>, <tbody>, <tfooter> - To cover header, body and the footer of the table. Won't change the appearance, but will give semantic meaning. 

** unlike other block level elements table do not take the whole space to the right.
** it takes enough to wrap the content inside.

<td> has attributes like colspan and rowspan to stretch columns and rows for more than one
** add <th> inside <tr> which already has <td> content to give a table heading on the left side. 
** use scope="" attribute inside the <th> tag to define if its a column heading or row heading
eg:- <th scope="col"> to headings that display 'Time' and 'Activity'
    <th scope="row"> to heading that display 'Morning', 'Noon', 'Afternoon'...

=======================================================================================
FORMS AND INPUT

<form> - to create a form to collect data from the user.
** by default it comes with action attribute, and we should give where we send data collected from this form.
** content inside forms are typically lables and input
<fieldset> - draws a box around the form
<legend> - caption the box
<label> - to describe the input to the user. 
** by default label gets for attribute in the tag. the for value should match the id value of the input tag
<input> - to get the actual data from the user.
** type - (text, button, checkbox..etc). 
        - type 'tel' for phone numbers. type 'number' will give two arrows up and down. 'tel' will give numbere pad for mobiles
        - type 'number' have min, max values, step (+ or - by how much), value (default value)
        - 'list' makes a list
        eg:- <input type="text" name="coffee" id="coffee" list="coffee-list">
        - radio gives a mcq type selection. 'name' attribute must be the same for every input
        - checkbox is pretty much the same as radio.
        - there cannot be id named 'other'/ or anyother same name to choices.

** name - attribute is what the serverside use to identify the tag. When we send data to the server, the data is labeld with the value in the name attribute.  
** id - is the id value of the tag.
** placeholder - is the string that displays inside the input window. its holding the place of whatever value will be put in. 
** autocomplete - 'on' or 'off' to suggest previously entered inputs. (not suppored for password type)
** required - to make it a required field on the form. doesnt need any value to it. 
** autofocus - when we load the page, it will be the first thing to get input, with the cursor attached to it.
                can be only used in one form input.
** pattern - to get input in a specific pattern. the input has to match that.

** id, and for(lable) should be identical
<select> - gives a dropdown selector with options.
         - select has 'name' and 'id' attribute like input. id should match for ( in lable)
         - 'multiple' attribute allows the user to pick multiple options.
         - 'size' will show that amount of options at once without dropdown in a scrollable menu. (it includes optgroup values.) 

<options> - options inside of a select dropdown.
          -'value' attribute to give value name.
          -'selected' attribute to mark an option as default selected.
<optgroup> - use to group options of the options.
           - 'label' attribute in optgroup will show as group heading.

<datalist> - creates a field to type and choices.
         <input type="text" name="coffee" id="coffee" list="coffee-list">        
    eg:- <datalist id="coffee-list">
            <option value="regular coffee">
        (list id and datalist id must be the same)
        (no closing tags in <option> in this)

<textarea> - to get a text box. 
            - 'cols' and 'rows' attributes

*** can use 'formaction' and 'formmethod' attributes inside <button> tag to use 'post' method instead of 'get' to send data.
<button type="submit" formaction="https://httpbin.org/post" formmethod="post">Post</button>

**** when submitting form data using 'get' or <input> <datalist> way, it shows the transmitted data inside the url. not safe. use POST for submitting data.
