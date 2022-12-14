```dataview
TABLE WITHOUT ID file.name AS OS, end_date
FROM "Informations"
SORT file.end_date DESC
WHERE startswith(file.name, "OS")
```

