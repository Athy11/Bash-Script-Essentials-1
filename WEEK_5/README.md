# DATA PROCESSING AND TEXT MANIPULATION
In data processing and text manipulation involves extracting useful information by filtering, modifying, and restructuring text data from files.

## EXTRACTING AND FILTERING DATA (GREP)
With the use of **grep**, one can extract and filter data. Grep is for searching text, it finds lines that match a pattern in a file.

| Command | Description |
| ----------- | ----------- |
| -i | Case-insensitive search |
| -n | Show line numbers with matches |
| -v | Invert match (show lines not matching) |
| -c | Count occurrences of a match |
| -o | Show only matching parts, not full lines |
| -E | Use extended regex (Egrep equivalent) |

## TEXT SUBSTITUTION AND EDITING (SED)
With the use of **sed**, substitution and editing text is possible.

| Command | Description |
| ----------- | ----------- |
| s/find/replace/ | Find and replace text |
| -i | Modify file in place (no output) |
| /pattern/d | Delete lines matching pattern |
| -n | Suppress default output (use with p) |
| p | Print only matching lines |

## COLUMN EXTRACTION AND PROCESSING (AWK)
With the use of **awk**, column extraction and processing is easy.

| Command | Description |
| ----------- | ----------- |
| -F | Set delimiter (field separator) |
| BEGIN {} | Run code before processing |
| {print $1} | Print specific column(s) |
| $2 > 20 | Filter rows based on condition |
| NR==3 | Print only the 3rd row |

## LET’S PRACTICE YOUR KNOWLEDGE

