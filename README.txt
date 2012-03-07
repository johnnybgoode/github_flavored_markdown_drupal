Github Flavored Markdown
==============================

Installation
------------------------------

1. Download and enable the Markdown module (http://drupal.org/project/markdown)
2. Enable the Github Flavored Markdown module
3. Create an Input Format and enable both the Markdown filter and the Github
   Flavored Markdown filter.
4. Visit the 'Rearrange' tab and ensure that the Github Flavored Markdown filter
   is placed before Markdown.
5. Optionally visit the 'Configure' tab and disable any features of Github
   Flavored Markdown that you do not need, for example if using Markdown Extra
   you may not need Github Flavored Markdown's fenced code functionality

Features
------------------------------

*Hard Wrap Newlines*
Treat single newlines in paragraph-like content as line breaks. This is
more intuitive for most users than the way in which Markdown normally handles
hard line breaks.

*Escape Underscores Inside Words*
It is unreasonable to italicize just part of a word, therefore words containing
multiple underscores are escaped. This is especially useful on sites where users
are entering code snippets, which very likely contain variables of the form
foo_bar_baz.

*Fenced Code Blocks*
Markdown supports the delineation of code blocks by beginning each line with at
least four spaces or a tab character. This can become cumbersome when entering
longer snippets, so Github Flavored Markdown implements fenced code blocks --
text surrounded by lines containing only three backticks (```). For example:
```
<?php
  print 'Hello World';
?>
```
is equivalent to
    <?php
      print 'Hello World';
    ?>

*Auto Linking of Raw URLs*
Github Flavored Markdown attempts to find raw URLs in the text and format them
as Markdown style links so they are later transformed into HTML anchor tags by
the Markdown processor.

Notes
------------------------------

All features of this module may be disabled from an Input Format's
'Configuration' tab. If your site uses a recent version of the Markdown modules
that leverages Michel Fortin's Markdown PHP / Markdown Extra, it may not be
necessary for the Github Flavored Markdown filter to preprocess fenced code
blocks or escape underscores in words.

If your site is experiencing problems, ensure that the Github Flavored Markdown
filter is placed _before_ the Markdown filter on the Input Format's 'Rearrange'
tab.
