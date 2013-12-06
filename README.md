lcov-latex
==========

LaTeX output from LCOV 

I needed line coverage information in LaTeX, but LCOV does not support latex output, and further, pandoc wasn't able do a nice html to LaTeX conversion from the LCOV html output.

The changes I've made are rather hackish; it should be relatively simple to roll the functionality into LCOV genhtml proper (accessible through a command line parameter), but the hack I did already does everything I need.

I'm making the hack available since I feel other people may also benefit from this functionality. If someone feels like cleaning it up and posting a patch to the LCOV project, I won't mind ^_^

Note that the output is a bunch of LaTeX snippets, not a single document; these snippets can be easily included in larger LaTeX documents using the \input{} primitive. This is by design, as flexibility is desired.
