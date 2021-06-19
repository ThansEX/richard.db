## Örnek Kod

```js
const VeriTabanı = require("Richard.db");
const db = new VeriTabanı();

// Veri Ayarlama
db.ayarla("veri1", "1");

// Veriyi Çekme
db.cek("veri1"); // Çıktı: 1
db.bul("veri1"); // Çıktı: 1

// Veriyi silme
db.sil("veri1");

db.cek("veri1"); // Çıktı: undefined çünkü veriyi sildik
db.kontrol("veri1"); // Çıktı: false çünkü veriyi sildik
db.bul("veri1"); // Çıktı: undefined çünkü veriyi sildik

db.ayarla("yaş", 20);
db.ekle("yaş", 1); // Yaş adlı veri 21 oldu
db.eksilt("yaş", 10); // Yaş adlı veri 11 oldu

db.ayarla("liste", [ "elma" ]);
db.degerekle("liste", "portakal"); // [ "elma", "portakal" ]

// Tüm verileri silme 
db.temizle();
```
 
Yapımcı: TheLord(Yusuf Göçer)

