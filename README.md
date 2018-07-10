Install
===============

Install it via composer by adding to composer.json:
```
"imunhatep/htmlawed": "dev-master"
```


HTMLawed is ...
===============

... a single-file, 45 kb PHP script that makes input text more secure, HTML standards-compliant, and 
suitable in general from the viewpoint of a web-page administrator, for use in the body of HTML, XHTML 
or XML documents. A simple HTMLTidy alternative, the htmLawed filter, processor, purifier, sanitizer, 
beautifier, etc., is highly customizable. 

It ensures that HTML tags are balanced and properly nested tags, neutralizes code that may be used 
for cross-site scripting (XSS) attacks, limits allowed HTML elements, attributes, or URL protocols, 
tidies the code, and so forth.

As such it may serve as an alternative to [HTMLtidy](http://en.wikipedia.org/wiki/HTML_Tidy) in a 
sanitation context.


This repository is ...
======================

... a derivative, which closely tracks [the original](http://www.bioinformatics.org/phplabware/internal_utilities/htmLawed/)
and may contain some additional tweaks and tugs for performance and/or filtering ability reasons.

Current extra features compared to the original:

* UTF-8 throughout: all HTML entity conversions are now performed in UTF-8 (instead of an arbitrary 
  codepage; of course this assumes you'll feed the bugger UTF-8 (or what should be treated as UTF-8 
  at least), as does its own test page.
* the test page accepts up to 10x larger inputs than the original test page (so you can run a test on 
  large chunks of copy through the form)



Links
=====

* The Original: http://www.bioinformatics.org/phplabware/internal_utilities/htmLawed/
* The SF site where the official Original Releases are available (no cvs/svn/... repository there, though, just releases): http://sourceforge.net/projects/htmlawed/
* HTMLawed against RSnake's XSS attack vectors: http://www.bioinformatics.org/phplabware/internal_utilities/htmLawed/rsnake/RSnakeXSSTest.htm

