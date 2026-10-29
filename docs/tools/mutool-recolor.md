# mutool recolor

The recolor command changes the colorspaces used in a PDF file.

	mutool recolor [options] file

The options are:

-c colorspace
: The desired colorspace used in the output document: gray (default), rgb or cmyk.

-o output file
: Use the specified filename for the output PDF file with altered colorspaces.

-r
: Remove any output intents present in the input file.

file
: Input file name. The input must be a PDF file.
