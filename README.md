Wikia
=========

**Wikia** is a Python library that makes it easy to access and parse
data from any `wikia website <https://www.wikia.com>`

Search a wikia, get article summaries, get data like links and images
from a page, and more. Wikipedia wraps the `Wikia API
<http://api.wikia.com/wiki/Wikia_API_Wiki>`__ so you can focus on using
wikia data, not getting it.

Was rewritten as the original wrapper didn't work for a project.

```Python

  from wikia import wikia
  print(wikia.summary("dancingline", "The_Time"))
  # The Time is the 1st normal mode level in Dancing Line.

  wikia.search("Runescape", "Forest")
  # returns a list of the search word
  time = wikia.page("dancingline", "The_Time")
  time.title
  # u'The Time'
  time.url
  # u'http://dancingline.wikia.com/wiki/The_Time'
  time.content
  # u'The Time is the 1st normal mode level in Dancing Line.'...

  wikia.set_lang("en") # English
  wikia.summary("Runescape", "Runes", sentences=1)
  # returns first sentence of the summery
```

Note: this library was designed for ease of use and simplicity, not for advanced use.

Installation
------------
Place the wikia folder in your project and follow the example above. see wikitest.py for example.
