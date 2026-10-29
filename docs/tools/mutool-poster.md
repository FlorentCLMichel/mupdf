# mutool poster

The poster command reads the input PDF file and for each page chops it
up into x by y pieces. Each piece becomes its own page in the output
PDF file. This makes it possible for each page to be printed upscaled
and can then be merged into a large poster.

	mutool poster [options] input.pdf [output.pdf]

The options are:

-p password
: Use the specified password if the file is encrypted.

-m margin
: Set the margin (overlap) between pages in points or percent.

-x x-factor
: How many horizontal columns to divide each page into.

-y y-factor
: How many vertical rows to divide each page into.

-r
: Split horizontally from right to left (default splits from left to right).

input.pdf
: The input PDF document.

output.pdf
: The output filename. Defaults to "out.pdf" if omitted.
