# Text to Emoji

Bu Python projesi, verilen bir metni emoji ile dönüştürmeye yarayan basit bir fonksiyon içerir. Belirli kelimeler, karşılık gelen emojilerle değiştirilir ve geri kalan metin olduğu gibi kalır.

## Özellikler

- Verilen metindeki belirli kelimeleri emojilerle değiştirme.
- Kelimeler, küçük harfe dönüştürülerek eşleşme yapılır.
- Eğer kelime sözlükte bulunamazsa, kelime olduğu gibi bırakılır.

## Kullanım

### Gerekli Kütüphaneler

Bu proje sadece Python'un dahili kütüphanelerine dayanır, ek bir kurulum gerektirmez.

### Fonksiyonlar

#### `text_to_emoji(text)`

- **Parametreler**: 
  - `text` (str): Dönüştürülmek istenen metin.
  
- **Dönüş Değeri**: 
  - Fonksiyon, verilen metni emoji ile dönüştürüp bir string olarak geri döndürür.

#### Örnek

```python
text = "The wizard and the alien found a new planet under the moon and stars."
print(text_to_emoji(text))
```

Çıktı:

```
The 🧙 and the 👽 found a new planet under the 🌙 and ⭐.
```

### Emoji Sözlüğü

Aşağıda, metni emojiye dönüştürürken kullanılan kelimeler ve karşılık gelen emojiler listelenmiştir:

- **cat**: 🐱
- **dog**: 🐶
- **sun**: ☀️
- **star**: ⭐
- **moon**: 🌙
- **wizard**: 🧙
- **robot**: 🤖
- **alien**: 👽
- **love**: ❤️
- **fire**: 🔥
- **earth**: 🌎
- **sky**: 🌌

### Çalışma Prensibi

1. `text_to_emoji` fonksiyonu, verilen metni kelimelere ayırır.
2. Her kelime, emoji sözlüğünde aranır.
3. Eğer sözlükte eşleşen bir emoji varsa, kelime bu emoji ile değiştirilir.
4. Eşleşmeyen kelimeler olduğu gibi metne eklenir.
5. Sonuç olarak, dönüştürülmüş metin bir string olarak döndürülür.

## Katkı

Bu projeye katkıda bulunmak isterseniz, önerilerinizi ve düzeltmelerinizi PR (pull request) olarak gönderebilirsiniz.
