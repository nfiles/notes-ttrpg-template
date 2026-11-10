
## campaigns
```dataview
TABLE choice(DM = this.file.link, "👑", "") AS DM,
      choice(contains(players, this.file.link), "✅", "") AS player
FROM "campaign"
WHERE contains(players, this.file.link)
   OR DM = this.file.link
SORT file.created DESC
```
## characters
```dataview
TABLE
FROM "pages"
WHERE contains(players, this.file.link)
```
