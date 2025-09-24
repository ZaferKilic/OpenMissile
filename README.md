<p align="center">
  <img src="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/PngLogoText.png?raw=true" />
</p>


<p align="center">
  <a href="https://www.buymeacoffee.com/c9cwcg6kpjt" target="_blank">
    <img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffe&emoji=&slug=c9cwcg6kpjt&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00" alt="Buy Me a Coffee" />
  </a>
</p>

https://img.shields.io/badge/%3Ca%20href%3D%22https%3A%2F%2Fwww.buymeacoffee.com%2Fc9cwcg6kpjt%22%3E%3Cimg%20src%3D%22https%3A%2F%2Fimg.buymeacoffee.com%2Fbutton-api%2F%3Ftext%3DBuy%20me%20a%20coffe%26emoji%3D%26slug%3Dc9cwcg6kpjt%26button_colour%3DFF5F5F%26font_colour%3Dffffff%26font_family%3DCookie%26outline_colour%3D000000%26coffee_colour%3DFFDD00%22%20%2F%3E%3C%2Fa%3E


<span> Model roketlerden gelen gerçek zamanlı verileri görselleştirip işleyebilen bir yer istasyonu ve test platformu. OpenMissile sayesinde, seri port üzerinden alınan veriler işlenerek doğru analizler ve sonuçlar elde edebilirsiniz. Ayrıca Teknofest Roket Yarışması'na katılan takımlar için özel ayrıcalıklar da sunmaktadır 🚀

## Son Güncelleme
Yeni güncellemede kullanıcı arayüzü optimizasyonlarını geliştirdim. Artık "Profil" sekmesinin altında uçuşlar listelenecek ve uçuş kaydına ait detaylı bilgi ekranı açılacak. Bu bilgi ekranında kullanıcılar geçmiş uçuşu simüle edebilecek ve roketin havadaki hareketlerini yeniden izleyebilecek.

<br>
<br> <a href="https://vimeo.com/999917068?share=copy">TANITIM VİDEOSU</a></span>

![Ana Ekran](https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Main.png?raw=true)
<a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Graphs.png"> Grafikler </a>
<a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Maps.png"> Haritalar </a>
<a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Profile.png"> Profil </a>
<a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Test.png"> SİT ve SUT </a>
<a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Settings.png"> Ayarlar </a>

## Özellikler
- Gerçek zamanlı veri görselleştirme
- Teknofest Roket Yarışmasında zorunlu olan SİT ve SUT testi
- 3D Simülasyon
- Harita üzerinde canlı konum takibi — <a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Maps.png">ÖRNEK</a>
- Sesli Uyarılar
- Rokete komut gönderme
- Roket ile yer istasyonu arasındaki mesafe hesaplama
- Veri iletim hızı ölçümü
- [BETA] Veri kaybı durumunda iniş noktası tahmini
- Roketten kamera görüntüsü izleyebilme
- Verileri uzaktaki bir sunucuya TCP ile gönderme
- Teknofest Roket Yarışması standartlarına uygun geliştirme
- Yer istasyonundan Teknofest roket yarışması hakemlerine veri iletimi
- Uçuş verilerini kayıt altına alma — <a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Profile.png">ÖRNEK</a>
- Özelleştirilebilir arayüz — <a href="https://github.com/ZaferKilic/OpenMissile/blob/main/Images/ScreenShots/Settings.png">ÖRNEK</a>

## Kullanım
OpenMissile, seri port üzerinden gelen verileri ayrıştırmak için JSON formatı kullanır. Her veri parçası, benzersiz anahtarlar ile ilgili alanlara yazılır.

Arduino tabanlı bir mikrodenetleyici kullanıyorsanız, aşağıdaki kütüphaneyi kullanabilirsiniz: <a href="https://github.com/bblanchon/ArduinoJson">ArduinoJson</a>.


## Kabul Edilen Veri Formatı
- OpenMissile içinde verilerin yazıldığı bölümlerin üzerine geldiğinizde, hangi anahtarın kullanıldığını görebilirsiniz.
- Kabul edilen veri örneği:



```
    {
    "SeaAlt": 123.00,
    "vSpeed": 123.00,
    "Temp": 123.00,
    "Pressure": 123.00,
    "X": 36.01,
    "Y": 76.01,
    "Z": 2.01,
    "AccX": 36.01,
    "AccY": 36.01,
    "AccZ": 36.01,
    "GForce": 36.01,
    "Apogee": 1500,
    "Latitude": 39.9250533,
    "Longitude": 32.8361282,
    "GpsAlt": 36.01,
}
```

## Lisans
This project is licensed under the MIT License. For more details, see the LICENSE file.
