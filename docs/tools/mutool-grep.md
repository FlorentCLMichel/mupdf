# mutool grep

The grep command searches for text in a document and prints each matching line.

	mutool grep [options] pattern file [ file2 ...]

The options are:

pattern
: A regular expression or string to search for.

file
: Document to search in.

-p password
: Use the specified password if the file is encrypted.

-F
: The pattern is a fixed string.

-a
: Ignore diacritics and accents (treat ä and a as the same).

-i
: Ignore case (treat A and a as the same).

-H
: Print filename for each match.

-n
: Print page number for each patch.

-S search-options
: See [search options](/reference/common/search-options).

-O stext-options
: See [structured text options](/reference/common/stext-options).

-b
: Search backwards, starting from the end.

-[ start-mark
: Insert mark at the start of each match when printing results.

-] end-mark
: Insert mark at the end of each match when printing results.

-v
: Show verbose search debugging feedback.

-q
: Hide all warnings and error messages. Use at your own risk!
