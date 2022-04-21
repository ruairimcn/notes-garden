# Obsidian Dataview
Dataview is a plugin for [[Obsidian]] that lets you write queries that act on your notes.
I currently use it for creating self-generaitng tables.

**Documentation:**  [Dataview Documentation](https://blacksmithgu.github.io/obsidian-dataview/docs/creating-queries)


# Code examples

```dataview
TABLE file.tags AS "Tags" FROM #Book
```


```dataview
TABLE date-of-birth AS "DOB" FROM #Contact
sort date-of-birth.month ASC, date-of-birth.day ASC
```

```dataview
TABLE Author, Genre, Rating FROM #Book
WHERE !contains(file.name, "Directory")
SORT Rating DESC
```

## Exclude based on path
` WHERE !contains(file.name, "Directory") `


---
**Links:** 
**Tags:** 

**Sources:**

**Created:** 2021-06-10  11:43