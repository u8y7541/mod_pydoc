# mod_pydoc
Attempt at modernizing the look of html pages served by pydoc

Pydoc is great - no, make that **fantastic**.
However, I (and apparently other people) do not like the choice of colors
for the pages served in a  browser by pydoc.

This fork has a custom css file which you can use to make pydoc look better.
To see it (u8y7541's css):

    python mod_pydoc.py -b -c custom.css

![screenshot](Screenshot01.png)
![screenshot](Screenshot02.png)

The original pydoc module has hard-coded values for color choices.
This new version, based on html5, uses css styling.

To test (aroberge's css):

    python mod_pydoc.py -b

To see a css close approximation of the original css:

    python mod_pydoc.py -b -c classic

To use a user-defined css file:

    python mod_pydoc.py -b -c <path_relative_to_cwd>

The file pydoc_test.css is included as an example of a very slightly
customized file (the background color is different from the new default).
To run it:

    python mod_pydoc.py -b -c pydoc_test.css
