# gdiu_webcontent

for some reason this has to be updated to get the served files to update....

Uses somewhat-correct XML as external resources.
All data is stored at the top level.

### Special tag formats used during injection:
- <*tag>e1, e2, e3</*tag> creates a tag list with comma-separated values
- <$tag>some.url</$tag> injected image element is given a src attribute 'some.url'
- <&tag>some.url</&tag> injected element is given a background image "url('some.url')"
- <@tag>formatted text</@tag> injected content is preprocessed according to formatting described below
- <~tag>text</~tag> injected element gains a value='text' attribute

### mu Preprocessor formating
- p(text) makes a paragraph of text
- =text= makes heading text
- *text* makes bold text
- _text_ makes italicized text
- #(some.url)[small tag1 tag2] makes an inline image with src 'some.url' and classes 'small tag1 tag2'
- [some.url][some text] makes a new-tab link to some.url with text 'some text'
- [=some.url][some text] makes a same-tab link to some.url with text 'some text'
- Two new-line characters will be replaced with a double &lt;br/&gt; (one newline will be ignored)
