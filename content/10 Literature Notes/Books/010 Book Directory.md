```dataview
TABLE Author, Genre, Rating, "![["+image+"]]" as Image FROM #Book
WHERE !contains(file.name, "Directory") OR !contains(file.name, "Template")
SORT Rating DESC
```


---
**Tags**:: #Personal/Directory

**Sources**::

**Date created**:: 2021-11-21  
**Time created**:: 16:29