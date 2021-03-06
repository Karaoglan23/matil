# Matil Nedir?

Matematiksel problemleri (sınav sorularını) çözmek amacına odaklanmış bir programlama dilidir.
Bu dil Python programlama dili ile geliştirilmiştir. Dosya uzantısı `.matil` olan dosyalar yorumlayici.py ile çalıştırılabilir.
Proje TYT soruları odağında olduğundan projeye bazı TYT soruları ve çözüm için gerekli olan kodları içeren dosyalar eklenilmiştir.
yorumlayici komut satırında parametre olmaksızın çalıştırıldığında yıllara göre konu ve soru seçip kod düzenleyip, soru seçimine izin veren bir komut satırı arayüzüne(cli) sahiptir.

# Ekip
numara | isim soyisim |
---|---|
195260068|Samet Karadağoğlu|
16260902|Abdulhadi Yılmaz|
10260059|Muhammed İrşad Özel |

# Örnek matil kodları

Kesirler
```
>>> kesir1 = Kesir(1, 3)
>>> yaz(kesir1)
1/3
>>> kesir2 = Kesir(2, 5)
>>> yaz(kesir2)
2/5
>>> yaz(kesir1 + kesir2)
11/15
```

Kümeler

```
>>> gizemli_kume = Kume(lambda kume : kume.elemanSayisi içinde kume)
>>> gizemli_alt_kume_listesi = Kume()
>>> A = Kume([1,2,3,4,5,6])
>>> Her altKume içinde A.tumAltKumeler():
>>>    Eğer(gizemli_kume.test(altKume)):
>>>        gizemli_alt_kume_listesi.ekle(altKume)
>>> yaz(gizemli_alt_kume_listesi.elemanSayisi)
32
```

Permutasyon

```
>>> yaz(Permutasyon(3, 2)) #3'ün 2'li permütasyonu
6
>>> list(Permutasyon([1,2,3], 2)) #dizinin 2'li permütasyonu
[(1, 2), (1, 3), (2, 1), (2, 3), (3, 1), (3, 2)]
```

Kombinasyon

```
>>> yaz(Kombinasyon(4, 1) * Kombinasyon(4, 3) * Kombinasyon(2, 1) * Kombinasyon(4, 2))
192
>>> kombinasyon = Kombinasyon([1,2,3,4,5,6], 2)
>>> yaz(kombinasyon)
15
>>> yaz(list(kombinasyon))
[(1, 2), (1, 3), (1, 4), (1, 5), (1, 6), (2, 3), (2, 4), (2, 5), (2, 6), (3, 4), (3, 5), (3, 6), (4, 5), (4, 6), (5, 6)]
```

Denklem

```
>>> x = Degisken('x')
>>> denklem = Denklem("x**2 = 1", [x])
>>> denklem.yaz()
x**2 = 1
>>> denklem.coz()
[-1, 1]
```