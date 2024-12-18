```dataview    
TABLE    
title as Title,     
FirstAuthor as "First Author",     
Year as Year,    
tags as Tag,     
summary as Summary    
FROM "zotero_notes"  
```



```dataview
TABLE without id 
  Progress_Bar AS "Progress Bar",
  ("![cover|80](" + Cover + ")") as Cover,
  file.link AS "Title",
  Author AS "Author",
  Category AS "Genre"
FROM #FM/📁02/📖 
where Status = "Currently-reading"
SORT Progress desc
```



