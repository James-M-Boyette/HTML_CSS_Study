# HTML

- Often, naming files with "index.html" is a good practice because ?browsers? look for this file by default in the root of a website's directory

- A page's head tag contains things like meta-data (Which i need to research more later), title etc

- "div" = "division"; html5's 'symantic' tags are replacing these generic ones

- "span" tags are intended to let you to insert CSS or JS into the html

- As of html5, tags that had no potential content within them (< br >, < hr >, < img >, etc.) no longer required "self-closing" slashes (< img />) and just need their vanilla instantiation (< img >)

- In < img > tags, the "alt" property allows you to provide text descriptions for screen readers (which wont display the actual image); it's an accessibility feature

- The "action" attribute in form tags will provide instructions on what to do with the data inputed

- The "type" attribute of a form's _input_ describes the expected data type to be received

# CSS

- To link individual HTML pages to specific CSS sheets, insert a < link > tag, and set its 'href' attribute to the relative path of the given style sheet.

  > Ex: < link rel="stylesheet" href="css/styles.css" >

- When using the color picker, you can click on the top bar to change the format (from rgb to hex/# etc)

- **Block-level** vs **inline** ...

  - The former will take up an entire line on their own, while the latter only take up the space their content requires (images, spans, links etc). You can also see this in the 'Elements' tab of a browser, where block-level page elements will have an attribute added called "display," which is set to "block" ... which means that you can convert in-line elements to block ones by setting their "display" property to block! (and vice-versa for block-level ones)

  - Morover, in-line elements don't automatically have top and bottom margin; they do have top and bottom padding, but when pages are re-sized, even their padding doesn't behave as normal and the space between two in-line elements is removed

- "**Margin Collapse**": when two elements have margin settings, but the greater value is chosen as the overall distance between them (two elements with top/bottom margins of 20px wont result in a space of 40px - only 20px, and two objects with 20 and 60px, respectively, will only have 60 pixels of space between them ...)

- "**Inline block**": mixes the two types such that

  1. it _wont_ go to a new line and take up the entire width of the page, but
  2. it _will_ have padding and margin all the way around (like a normal block element)

- "**Default Browser styles**": an accessibility feature, this is what makes HTML tags have the 'out-of-the-box' stylings that they have (h tags are bigger and bolder, list items have 'disc' bullet points, etc.). "User agent stylesheet" represents the rules asserted by the browser.

- IDs are, according to Sean, mainly used for JS - they _can_ be used for CSS, but it's preferred that one use \_

- If you want to quickly fill an element with "Lorem Ipsum" text, type `lorem`

- "**Cascading / Inheritance**": some CSS properties are passed on to children (like font styling), while others are not (padding, margin, etc.). If you'd like normally-uninherited properties to be passed on to child elements, you need set the given child's uninherited property to "inherit" (`margin: inherit`)
