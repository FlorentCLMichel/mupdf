# mutool trim

This command allows you to make a modified version of a PDF with content
that falls inside or outside of various "boxes" removed.

See [mutool pages](/tools/mutool-pages.md) for how to list out the boxes used on a page.

	mutool trim [options] input.pdf

The options are:

-b box
: Which page box to trim to (mediabox (default), cropbox, bleedbox, trimbox, artbox).

-f
: Fallback to mediabox if specified box not available.

-m margins
: Add margins to box (positive for inwards, negative for outwards).
: One number for all margins, or two for vertical and horizontal, or
four for T,R,B,L respectively.

-e
: Exclude contents of box, rather than include them.

-o filename
: Output file.

## Examples

Trim a document by trimming the MediaBox elements with a margin of 200
points inwards:

	mutool trim -b mediabox -m 200 -o out.pdf in.pdf

Trim a document by trimming the MediaBox elements with a margin of 20
points from the top & bottom (vertical) and 30 points from the left &
right (horizontal):

	mutool trim -b mediabox -m 20,30 -o out.pdf in.pdf

Trim a document by trimming the MediaBox elements to a box offset 10
points from the top & right, 50 points from the bottom and 20 points in
from the left:

	mutool trim -b mediabox -m 10,10,50,20 -o out.pdf in.pdf

Exclude the contents of the ArtBox element:

	mutool trim -b artbox -e -o out.pdf in.pdf
