## Find lines from file A (exact string) that is not in file B

**Remove <CR>, if any**

tr -d '\r' < file

**Remove empty lines in a text file via grep**
grep . FILE > a_output.txt

**Remove tabs/spaces**

cat a.txt | tr -d '[[:blank:]]' > a_out.txt

**Do the comparison**
comm -23 a_out.txt b_out.txt

By default, comm outputs 3 columns: left-only, right-only, both. The -1, -2 and -3 switches suppress these columns.
So, -23 hides the right-only and both columns, showing the lines that appear only in the first (left) file


Reference
* http://stackoverflow.com/questions/14473090/find-lines-from-a-file-which-are-not-present-in-another-file
* http://stackoverflow.com/questions/1611809/remove-empty-lines-in-a-text-file-via-grep
