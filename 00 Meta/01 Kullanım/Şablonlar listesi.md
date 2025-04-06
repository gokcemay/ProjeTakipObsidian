Sistemin işlemesi için hazırlanmış olan şablonların listesi aşağıda verilmiştir. Bu şablonlarda değişiklikler yaparak özelleştirmeniz mümkündür. 
``` dataview
table file.name as "Dosya Adı", file.path as "Dosya Yolu"
from "00 Meta/02 Şablonlar"  // İlgili klasör yolunu buraya yazın
where contains(file.tags, "#şablon")
sort file.name asc

```
