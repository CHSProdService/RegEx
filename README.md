# RegEx
The Regular Expressions used in DFO's WET4 / web development.

**Please be aware that regular expressions can be dangerous to run en masse, be aware of the scripts you are running!**

## How To
To use these .dwr files simply open the find/replace window in Dreamweaver and click the "**Load Query**" button just above the find area on the right.

To save a new query or over write an existing one, click the "**Save Query**" button to the left of the "**Load Query**" button

## breadcrumbActive
The **breadcrumbActive.dwr** script is used to find the last list item of a breadcrumb and add active class to it as a design improvement.

### Example
**Before:**

    <li><a href='parent.html'>Parent</a></li><li>Child (current page)</li>
    
**After:**

    <li><a href='parent.html'>Parent</a></li><li class='active'>Child (current page)</li>
    
**This script is used only for sites that use the Breadcrumb variable**
    
## glyphicon-download
The **glyphicon-download.dwr** script is used to add the download glyphicon before any link that leads to a downloadable file.

Works on:

+ .doc
+ .docx
+ .xls
+ .xlsx
+ .ppt
+ .pptx
+ .pptm
+ .pdf
+ .zip
+ .rar

### Example
**Before:**

    <a href="download.pdf">PDF Document</a>
    
**After:**

    <span class="glyphicon glyphicon-download"></span> <a href="download.pdf"">PDF Document</a>
    
## glyphicon-email
The **glyphicon-email.dwr** script is used to add the envelope glyphicon to mailto links.

### Example
**Before:**

    <a href="mailto:me@email.com">me@email.com</a>
    
**After:**

    <span class="glyphicon glyphicon-envelope"></span> <a href="mailto:me@email.com">me@email.com</a>
    
## latinNamesItalics
This **latinNamesItalics.dwr** script is used to italicize known latin names for species.

### Example
**Before:**

    <p>Sebastes fasciatus</p>
    
**After:**

    <p><em>Sebastes fasciatus</em></p>
    
## dfoLinkFinder
The **dfoLinkFinder.dwr** finds any link that uses a web address from dfo-mpo.gc.ca. This is useful more so on files within dfo-mpo.gc.ca to help find links that should start with a / and not http.

### Example
**Will find:**

+ href="http://www.dfo-mpo.gc.ca/
+ href="http://dfo-mpo.gc.ca/
+ href="http://wwwstg.ncr.dfo-mpo.ca/
+ href="http://wwwdev.ncr.dfo-mpo.ca/