### **🌪️**

### **Proje Gereksinimleri: Atlantik Kasırgaları Analizi**

---

### **1. Hasar Verilerini Güncelleme**

- Elinizde 34 kategori 5 Atlantik kasırgasının toplam zararlarını içeren bir damages listesi var.
- Bazı kayıtlar "Damages not recorded" olarak geçerken, diğerleri "10B" veya "500M" gibi yazımlarla milyar ya da milyon USD cinsinden belirtilmiş.
- Bu veriler üzerinde çalışabilmek için:
    - "B" (milyar) → 1000000000
    - "M" (milyon) → 1000000
- Bir fonksiyon yazın ve her veriyi float değere dönüştürün. "Damages not recorded" olduğu gibi kalsın.
- damages verisi ile fonksiyonu test edin.

---

### **2. Kasırga Verilerini Sözlük Haline Getirme**

- Elinizde 6 farklı liste var:
    - names, months, years, max_sustained_winds, areas_affected, deaths
- Her listedeki indeksler aynı kasırgaya ait bilgileri temsil eder.
- Bu verileri kullanarak:
    - Anahtarları kasırga adları olan bir sözlük oluşturun.
    - Her kasırga ismine karşılık gelen değer, bilgileri içeren başka bir sözlük olsun.
- Örnek:

```
{
  "Cuba I": {
    'Name': 'Cuba I',
    'Month': 'October',
    'Year': 1924,
    'Max Sustained Wind': 165,
    'Areas Affected': [...],
    'Damage': ...,
    'Deaths': ...
  }
}
```

---

### **3. Kasırgaları Yıllara Göre Gruplama**

- Önceki sözlüğü kullanarak yeni bir sözlük oluşturun:
    - Anahtarlar yıl olacak.
    - Değerler, o yıl yaşanan kasırgaların sözlükleri içeren listeler olacak.
- Örnek:

```
{
  1932: [
    {hurricane_1_dict},
    {hurricane_2_dict}
  ]
}
```

---

### **4. Etkilenen Bölgelerin Sayımını Yapma**

- Her kasırganın etkilediği bölgeleri analiz edin.
- Her bölgenin kaç kez etkilendiğini sayan bir sözlük oluşturun:
    - Anahtarlar bölgeler, değerler etki sayısı olacak.

---

### **5. En Fazla Etkilenen Bölgeyi Bulma**

- Önceki adımdaki sözlükten:
    - En çok etkilenen bölgeyi ve kaç kez etkilendiğini bulun.

---

### **6. En Çok Ölümle Sonuçlanan Kasırgayı Bulma**

- Kasırga sözlüğünden:
    - En fazla ölüme yol açan kasırgayı ve ölüm sayısını bulun.

---

### **7. Ölümcüllüğe Göre Kasırga Derecelendirmesi**

- Aşağıdaki mortality_scale kullanılarak kasırgaları derecelendirin:

```
mortality_scale = {
  0: 0,
  1: 100,
  2: 500,
  3: 1000,
  4: 10000
}
```

- Her derecelendirme için bir anahtar olacak, değeri o sınıfa giren kasırga sözlüklerinden oluşan bir liste olacak.

---

### **8. En Büyük Zarara Yol Açan Kasırgayı Bulma**

- Sözlükten, en fazla maddi hasara yol açan kasırgayı ve zarar miktarını bulun.

---

### **9. Zarara Göre Kasırga Derecelendirmesi**

- Aşağıdaki damage_scale kullanılarak maddi zarara göre kasırgaları sınıflandırın:

```
damage_scale = {
  0: 0,
  1: 100_000_000,
  2: 1_000_000_000,
  3: 10_000_000_000,
  4: 50_000_000_000
}
```

- Her derecelendirme için bir anahtar olacak, değeri o sınıfa giren kasırga sözlüklerinden oluşan bir liste olacak.

---

### **✅**

### **10. Çözümünü Paylaş**

- Projeni tamamladın!
- **Codecademy forumlarında** örnek çözümle karşılaştırabilir, istersen çözümünü GitHub’da yayınlayabilirsin.
- Farklı çözümler mümkündür, seninkinin farklı olması tamamen doğaldır.

---

🔍 **Hazırsan, şimdi her bir adımı tek tek kodlamaya başlayabilirsin!** Yardım istersen buradayım.
