# Gömülü Sistemler Kartı

YouTube'daki **Gömülü Sistemler** serisinde sıfırdan tasarladığımız ATmega328PB tabanlı, Arduino uyumlu genel amaçlı geliştirme kartı.
Şematikten PCB'ye, üretimden programlamaya kadar her adım seride anlatılıyor.

- Bölümler: [burakkaanboyuk.com/liste.html?k=gomulu-sistemler](https://burakkaanboyuk.com/liste.html?k=gomulu-sistemler)

## Kartta neler var

- **MCU:** ATmega328PB, 16 MHz kristal, Arduino IDE ile programlanabilir
- **Güç:** 5 V giriş, AMS1117-3.3 ile 3,3 V; ters gerilim koruması
- **Giriş / çıkış:** optokuplörlü iki giriş, transistörle sürülen röle çıkışı, fan kontrolü
- **Sensör ve haberleşme:** TMP1075 I²C sıcaklık sensörü, I²C / SPI / programlama konnektörleri; LED'ler ve bir buton

## Klasörler

| Klasör | İçerik |
|---|---|
| `hardware/` | KiCad projesi (şematik, PCB, BOM) |
| `firmware/` | Örnek kodlar (bölümler ilerledikçe) |
| `docs/` | Şematik PDF ve görseller |

Gerber, drill, STEP ve şematik PDF gibi üretim dosyaları depoda tutulmaz; her sürümün **Releases** sayfasında bulunur.

## Açmak için

Proje **KiCad 10** ile hazırlandı. Daha eski sürümler dosyaları açamaz; KiCad kurmadan bakmak için Releases'teki şematik PDF'i kullanabilirsiniz.

Tüm semboller ve footprint'ler KiCad'in kendi kütüphanelerinden; ek kütüphane gerekmez.

## Röle çıkışı hakkında

Bu kart eğitim amaçlıdır. Röle çıkışını şebeke gerilimiyle (230 V AC) kullanmadan önce rölenin ve klemensin değerlerini, kart üzerindeki yalıtım mesafelerini kendiniz kontrol edin. Şebeke gerilimiyle çalışmak hayati tehlike taşır.

## Lisans

| Kapsam | Lisans |
|---|---|
| Donanım (`hardware/`) | [CERN-OHL-P-2.0](LICENSE) |
| Yazılım (`firmware/`) | [MIT](LICENSES/MIT.txt) |
| Doküman ve görseller (`docs/`, bu dosya) | [CC BY 4.0](LICENSES/CC-BY-4.0.txt) |

© 2026 Burak Kaan Böyük
