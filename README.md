# 📚 İleri Programlama Teknikleri

Bu repo "YMH220-İleri Programlama Teknikleri" dersimizin Github Clasroom çalışma ortamına aittir.

Bu GitHub deposu, "İleri Programlama Teknikleri" dersi için Python alıştırmalarını içermektedir. 
Bu alıştırmalar, Python'da list, tuple, string, dictionary gibi veri yapılarını kullanma becerilerinizi geliştirmenize ve algoritma yeteneğinizi ilerletmenize yardımcı olacaktır.

## 🎯 Talimatlar

1. Bu depoya (repository) Github Classroom assignment daveti ile ulaştınız, kendi hesabınıza fork edebilirsiniz.
2. Fork ettiğiniz depoyu bilgisayarınıza klonlayabilirsiniz
3. Her bir alıştırmayı ilgili Python dosyasında çözmelisiniz
4. Çözümlerinizi kendi fork'unuza push edin, ya da github üzerindeki repoya ekleyip commit ederek, assignment içine submit edebilirsiniz.

## ⚠️ Önemli Kurallar

- Çözümlerinizi Python 3.x kullanarak yazın
- Kodunuzda açıklayıcı yorumlar kullanın ve anlamlı değişken isimleri seçin
- Gereksiz kod tekrarından kaçının ve mümkün olduğunca verimli çözümler üretin
- Her bir alıştırma için belirtilen dosyayı kullanın (ornek1.py, ornek2.py, vb.)
- Kodunuzun hatasız çalıştığından emin olun

---

## 🧩 Alıştırmalar

### Alıştırma 1: Kelime Frekans Analizi 📊

Bir metin içinde geçen her kelimenin frekansını (kaç kez geçtiğini) hesaplayan bir program yazın. 
Program, kullanıcıdan bir metin almalı ve her kelimenin kaç kez geçtiğini frekans sırasına göre (en çok geçenden en az geçene) listelemelidir. 
Program noktalama işaretlerini dikkate almamalı ve büyük/küçük harf ayrımı yapmamalıdır.

**Örnek Çıktı:**
```
Metin girin: Merhaba dünya, merhaba Python! Python ile programlama yapmak çok eğlenceli.

Kelime frekansları:
python: 2
merhaba: 2
ile: 1
programlama: 1
yapmak: 1
çok: 1
eğlenceli: 1
dünya: 1
```

**İpucu:** String metodları, dictionary ve sorted() fonksiyonu kullanabilirsiniz.

**Dosya:** ex001.py

### Alıştırma 2: Matris İşlemleri 🔢

İki matris için toplama, çıkarma ve çarpma işlemlerini gerçekleştiren fonksiyonlar yazın. 
Matrisler, liste içinde liste (iç içe listeler) olarak temsil edilecektir. 
Programınız şu işlemleri yapabilmelidir:

1. İki matrisi topla
2. İki matris arasında çıkarma işlemi yap
3. İki matrisi çarp
4. Bir matrisin transpozunu bul

Ayrıca, programınız matris boyutlarının uyumlu olup olmadığını kontrol etmeli ve uygun hata mesajları vermelidir.

**Örnek Çıktı:**
```
Matris A:
[1, 2, 3]
[4, 5, 6]

Matris B:
[7, 8, 9]
[10, 11, 12]

A + B:
[8, 10, 12]
[14, 16, 18]

A - B:
[-6, -6, -6]
[-6, -6, -6]

A x B: (3x3 boyutunda olmadığı için çarpım yapılamaz)
Hata: Matris çarpımı için ilk matrisin sütun sayısı, ikinci matrisin satır sayısına eşit olmalıdır.

A'nın Transpozu:
[1, 4]
[2, 5]
[3, 6]
```

**İpucu:** İç içe listeler (nested lists) ve matris işlemleri algoritmaları kullanın.

**Dosya:** ex002.py

### Alıştırma 3: Öğrenci Not Sistemi 📝

Bir öğrenci not sistemini simüle eden bir program yazın. 
Program şu özelliklere sahip olmalıdır:

1. Öğrencileri ve notlarını bir dictionary içinde saklayabilmeli (öğrenci numarası anahtar, notlar ve bilgiler değer olarak)
2. Yeni öğrenci ekleyebilmeli
3. Mevcut öğrencinin notlarını güncelleyebilmeli
4. Öğrencileri numaraya veya ortalama nota göre listeleyebilmeli
5. Belirli bir not aralığındaki öğrencileri bulabilmeli
6. Sınıf ortalamasını hesaplayabilmeli

Her öğrenci için ad, soyad, vize notu ve final notu bilgilerini saklayın. Ortalama, vize notunun %40'ı ve final notunun %60'ı alınarak hesaplanmalıdır.

**Örnek Veri Yapısı:**
```python
ogrenciler = {
    "123456": {
        "ad": "Ahmet",
        "soyad": "Yılmaz",
        "vize": 75,
        "final": 85
    },
    "234567": {
        "ad": "Ayşe",
        "soyad": "Kaya",
        "vize": 90,
        "final": 95
    }
}
```

**İpucu:** Dictionary işlemleri, koşullu ifadeler ve fonksiyonlar kullanın.

**Dosya:** ex003.py

### Alıştırma 4: Dosya İşleme ve Veri Analizi 📊

Bir CSV dosyasından veri okuyup analiz eden bir program yazın. Programınız şu işlevlere sahip olmalıdır:

1. Verilen bir CSV dosyasını okuma
2. Verileri belirli bir sütuna göre sıralama
3. Belirli bir sütunun minimum, maksimum ve ortalama değerlerini hesaplama
4. Verileri belirli bir kritere göre filtreleme
5. Analiz sonuçlarını yeni bir CSV dosyasına yazma

CSV dosyası, örneğin şu formatta olabilir:
```
id,ad,soyad,yas,maas
1,Ali,Yılmaz,35,10000
2,Ayşe,Demir,28,12000
3,Mehmet,Kaya,42,15000
4,Zeynep,Çelik,30,11500
```

**İpucu:** CSV modülü, dosya işlemleri (open, read, write) ve list işlemleri kullanın.

**Dosya:** ex004.py

### Alıştırma 5: Metin Şifreleme ve Çözme 🔐

Basit bir şifreleme ve çözme sistemi oluşturun. İki farklı şifreleme algoritması uygulayın:

1. **Sezar Şifrelemesi**: Her harfi alfabede belirli bir sayı kadar ileriye kaydırma.
2. **Anahtar Kelime Şifrelemesi**: Bir anahtar kelimeye göre harfleri değiştirme.

Programınız kullanıcıdan bir metin ve bir anahtar (sayı veya kelime) almalı, ardından şifreleme veya çözme işlemi gerçekleştirmelidir. 
Program hem metinleri şifreleyebilmeli hem de şifrelenmiş metinleri çözebilmelidir.

**Örnek Çıktı (Sezar Şifrelemesi):**
```
İşlem seçin (1: Şifrele, 2: Çöz): 1
Metni girin: Merhaba Dünya
Anahtar sayıyı girin (1-25): 3
Şifrelenmiş metin: Phukded Gxqbd
```

**Örnek Çıktı (Anahtar Kelime Şifrelemesi):**
```
İşlem seçin (1: Şifrele, 2: Çöz): 1
Metni girin: Merhaba Dünya
Anahtar kelimeyi girin: PYTHON
Şifrelenmiş metin: Hmcjyby Xüpuy
```

**İpucu:** String işlemleri, ASCII değerleri (ord(), chr()) ve karakter haritalama kullanın.

**Dosya:** ornek005.py

---

## 🤝 Yardım Alma

Sorularınız veya yardıma ihtiyacınız olduğunda:
- Ders materyallerini gözden geçirin
- Sınıf arkadaşlarınızla tartışın (ancak doğrudan kod paylaşmayın)
- Ofis saatlerini kullanın

Başarılar! 💻
