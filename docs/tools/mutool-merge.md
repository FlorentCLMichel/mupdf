# mutool merge

The merge command is used to pick out pages from two or more files and
merge them into a new output file.

	mutool merge [-o output.pdf] [-O options] ( input.pdf [pages] )+

The options are:

-o output.pdf
: The output filename. Defaults to "out.pdf" if not supplied.

-O options
: See [PDF write options](/reference/common/pdf-write-options).

input.pdf
: The first document.

pages
: Comma-separated list of page ranges to include from the first document.
The first page is "1", and the last page is "N".
If the page-list is omitted the default is "1-N".

You may add as many additional input and page-list pairs as required to merge multiple documents.
