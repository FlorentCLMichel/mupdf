# mutool convert

The convert command converts an input file into another format.

	mutool convert [options] file [pages]

The options are:

-p password
: Use the specified password if the file is encrypted.

-o output
: The output file name. The output format is inferred from the output
filename. Embed `%d` in the name to indicate the page number (for
example: `page%d.png`). Printf modifiers are supported, for example
`%03d`. If no output is specified, the output will go to standard output.

-F output format
: Default output format is inferred from output file name.

	raster
	: cbz, png, pnm, pgm, ppm, pam, pbm, pkm.

	print-raster
	: pcl, pclm, ps, pwg.

	vector
	: pdf, svg.

	text
	: html, xhtml, text, stext.

-O comma-separated list of options for output format
: See [PDF write options](/reference/common/pdf-write-options.md) and
[document writer options](/reference/common/document-writer-options.md).

-b box
: Use named page box (MediaBox, CropBox, BleedBox, TrimBox, or ArtBox).

-A bits
: Specify how many bits of anti-aliasing to use. The default is 8.

-W width
: Page width in points for EPUB layout.

-H height
: Page height in points for EPUB layout.

-S size
: Font size in points for EPUB layout.

-U filename
: User CSS stylesheet for EPUB layout.

-X
: Disable document styles for EPUB layout.

file
: Input file name. The file can be any of the supported input formats.

[pages]
: Comma-separated list of page ranges. The first page is "1", and the last page is "N". The default is "1-N".
