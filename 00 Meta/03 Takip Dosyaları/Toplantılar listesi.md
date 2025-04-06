```dataview
table Tarih as "Tarih"
from "10 Projeler"
where contains(file.tags, "#toplantı")
sort Tarih asc
```
