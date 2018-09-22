# gdiu_webcontent

for some reason this has to be updated to get the served files to update....

Uses somewhat-correct XML as external resources.
All data is stored at the top level.

### mu Preprocessor formating
- ((text)) makes a paragraph of text
- ==text== makes heading text
- \*\*text\*\* makes bold text
- \_\_text\_\_ makes italicized text
- #(some.url)\[small tag1 tag2] makes an inline image with src 'some.url' and classes 'small tag1 tag2'
- [some.url][some text] makes a new-tab link to some.url with text 'some text'
- \[=some.url]\[some text] makes a same-tab link to some.url with text 'some text'
- Two new-line characters will be replaced with a double &lt;br/&gt; (one newline will be ignored)
