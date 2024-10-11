# 1. Lister toutes les notes

```dataview
LIST 
```

s'obtient avec le code :

````
```dataview
LIST 
```
````

# 2. Lister les notes qui concernent des outils

```dataview
LIST FROM #outil
```

s'obtient avec le code :

````
```dataview
LIST FROM #outil
```
````

# 3. Lister les prochains cours

```dataview
LIST
WHERE Date >= date(today)
```

s'obtient avec le code :

````
```dataview
LIST
WHERE Date >= date(today)
```
````

# 4. Afficher les cours dans un calendrier

```dataview
CALENDAR Date
FROM #cours AND "Notes"
```

s'obtient avec le code :

````
```dataview
CALENDAR Date
FROM #cours AND "Notes"
```
````

# 5. Reproduire ce tableau

```dataview
TABLE WITHOUT ID
Date, file.link AS Cours, Enseignant
FROM "Notes" AND #cours
SORT Date ASC
```

s'obtient avec le code :

````
```dataview
TABLE WITHOUT ID
Date, file.link AS Cours, Enseignant
FROM "Notes" AND #cours
SORT Date ASC
```
````