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

===================================================================================
IMAGES
