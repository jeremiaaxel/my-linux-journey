```dataview
TABLE WITHOUT ID file.name AS Issues, is_solved
FROM "Issues"
SORT file.date DESC
WHERE !startswith(file.name, "TEMPLATE")
```

