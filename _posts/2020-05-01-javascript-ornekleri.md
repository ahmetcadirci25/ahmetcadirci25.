---
title      : "JavaScript Örnekleri"
description: "JavaScript dilinin çeşitli tekniklerini ve özelliklerini gösteren kapsamlı bir uygulamalı JavaScript örnekleri içerir."
date       : 2020-05-01 20:00:00
categories : [Kod, Program]
tags       : [JavaScript Örnekleri, JavaScript Örnekleri Basit, JavaScript Kod Örnekleri, JavaScript Uygulamaları]
image      : "/images/javascript-ornekleri.png"
comments   : true
---

JavaScript dilinin çeşitli tekniklerini ve özelliklerini gösteren kapsamlı bir uygulamalı JavaScript örnekleri içerir. 

Örnek kodları [Sublime Text 3]({{site.url}}/sublime-text-3/) kod editörü kullanarak deneyebilirsiniz. Ya da [gerçek zamanlı online HTML editörü]({{site.url}}/htmleditor/) kullanabilirsiniz.

**Sık sık örnekler güncellenecektir.**

## İçindekiler

- [JavaScript “Merhaba Dünya!” Uygulaması]({{site.url}}/2020/javascript-ornekleri/#javascript-merhaba-dünya-uygulaması)
- [JavaScript Kodunu Bir HTML Dosyasına Gömme]({{site.url}}/2020/javascript-ornekleri/#javascript-kodunu-bir-html-dosyasına-gömme)
- [HTML Belgesinde Harici Bir JavaScript Dosyası Çağırma]({{site.url}}/2020/javascript-ornekleri/#html-belgesinde-harici-bir-javascript-dosyası-çağırma)
- [HTML Etiketine JavaScript Kodu Ekleme]({{site.url}}/2020/javascript-ornekleri/#html-etiketine-javascript-kodu-ekleme)
- [JavaScript’te Büyük / Küçük Harf Duyarlılığı]({{site.url}}/2020/javascript-ornekleri/#javascriptte-büyük--küçük-harf-duyarlılığı)
- [JavaScript Tekli Yorum Satırı]({{site.url}}/2020/javascript-ornekleri/#javascript-tekli-yorum-satırı)
- [JavaScript Çoklu Yorum Satırı]({{site.url}}/2020/javascript-ornekleri/#javascript-çoklu-yorum-satırı)
- [JavaScript’te Değişken Oluşturma]({{site.url}}/2020/javascript-ornekleri/#javascriptte-değişken-oluşturma)
- [JavaScript’te Değişken Bildirme]({{site.url}}/2020/javascript-ornekleri/#javascriptte-değişken-bildirme)
- [Aynı Anda Birden Çok Değişkeni Bildirme]({{site.url}}/2020/javascript-ornekleri/#aynı-anda-birden-çok-değişkeni-bildirme)
- [Tarayıcı Konsoluna Yazma]({{site.url}}/2020/javascript-ornekleri/#tarayıcı-konsoluna-yazma)
- [Bir Uyarıyı İletişim Kutusuna Yazma]({{site.url}}/2020/javascript-ornekleri/#bir-uyarıyı-i̇letişim-kutusuna-yazma)
- [Tarayıcı Penceresine Yazma]({{site.url}}/2020/javascript-ornekleri/#tarayıcı-penceresine-yazma)
- [document.write() Yöntemle İlgili Sorun]({{site.url}}/2020/javascript-ornekleri/#documentwrite-yöntemle-i̇lgili-sorun)
- [HTML Öğesine Yazdırma]({{site.url}}/2020/javascript-ornekleri/#html-öğesine-yazdırma)
- [JavaScript’te Gerçek API ile Bağlantı Kurma ve Veri Çekme]({{site.url}}/2020/javascript-ornekleri/#javascriptte-gerçek-api-ile-bağlantı-kurma-ve-veri-çekme)
- [JavaScript’te Attribute Kullanarak Öznitelikleri Değiştirme]({{site.url}}/2020/javascript-ornekleri/#javascriptte-attribute-kullanarak-öznitelikleri-değiştirme)
- [JavaScript’te Click Event Kullanarak Kutuları Gizleme]({{site.url}}/2020/javascript-ornekleri/#javascriptte-click-event-kullanarak-kutuları-gizleme)

#### JavaScript "Merhaba Dünya!" Uygulaması

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript "Merhaba Dünya!" Uygulaması</title>
</head>
<body>

    <script>
        let merhaba = "Merhaba Dünya!";
        console.log(merhaba);
    </script>

    <p>Not: Klavyedeki F12 tuşuna basarak tarayıcı konsoluna (console) bakın.</p>

</body>
</html>
```

#### JavaScript Kodunu Bir HTML Dosyasına Gömme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript Kodunu Bir HTML Dosyasına Gömme</title>
</head>
<body>

    <script>
        let merhaba = "Merhaba Dünya!";
        document.write(merhaba);
    </script>

</body>
</html>
```

#### HTML Belgesinde Harici Bir JavaScript Dosyası Çağırma

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>HTML Belgesinde Harici Bir JavaScript Dosyası Çağırma</title>
</head>
<body>

    <button type="button" id="Btn">Tıkla</button>

    <script src="/js/main.js"></script>

</body>
</html>
```

#### HTML Etiketine JavaScript Kodu Ekleme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>HTML Etiketine JavaScript Kodu Ekleme</title>
</head>
<body>

    <button onclick="alert('Merhaba Dünya!')">Tıkla</button>

</body>
</html>
```

#### JavaScript'te Büyük / Küçük Harf Duyarlılığı

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript'te Büyük / Küçük Harf Duyarlılığı</title>
</head>
<body>

    <script>
        let merhabaDunya = "Merhaba Dünya!";

        console.log(merhabaDunya);
        console.log(MerhabaDunya);
        console.log(merhabadunya);
    </script>

    <p>Not: Klavyedeki F12 tuşuna basarak tarayıcı konsoluna (console) bakın, şöyle bir satır göreceksiniz: "Uncaught ReferenceError: merhabaDunya is not defined".</p>

</body>
</html>
```

#### JavaScript Tekli Yorum Satırı

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript Tekli Yorum Satırı</title>
</head>
<body>

    <script>
        // Bu benim ilk JavaScript örneğim
        document.write("Merhaba Dünya!");
    </script>

</body>
</html>
```

#### JavaScript Çoklu Yorum Satırı

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript Çoklu Yorum Satırı</title>
</head>
<body>

    <script>
        /* Bu benim ilk 
        JavaScript örneğim */
        document.write("Merhaba Dünya!");
    </script>

</body>
</html>
```

#### JavaScript'te Değişken Oluşturma

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript'te Değişken Oluşturma</title>
</head>
<body>

    <script>
        // Değişkenler Oluşturma
        let isim = "Mecnun";
        let yas = 21;
        let evliMi = false;
        
        // Değişken Değerlerini Yazdırma
        document.write(isim + "<br>");
        document.write(yas + "<br>");
        document.write(evliMi);
    </script>

</body>
</html>
```

#### JavaScript'te Değişken Bildirme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript'te Değişken Bildirme</title>
</head>
<body>

    <script>
        // Değişken Bildirimi
        let kullaniciAdi;
        
        // Değer Atama
        kullaniciAdi = "Leyla Mecnun";
        
        // Değişken Değerini Yazdırma
        document.write(kullaniciAdi);
    </script>

</body>
</html>
```

#### Aynı Anda Birden Çok Değişkeni Bildirme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Aynı Anda Birden Çok Değişkeni Bildirme</title>
</head>
<body>

    <script>
        // Birden Çok Değişken Bildirme
        var isim = "Mecnun", yas = 21, evliMi = false;
        
        // Değişken Değerlerini Yazdırma
        document.write(isim + "<br>");
        document.write(yas + "<br>");
        document.write(evliMi);
    </script>

</body>
</html>
```

#### Tarayıcı Konsoluna Yazma

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Tarayıcı Konsoluna Yazma</title>
</head>
<body>

    <script>
        // Basit bir metin mesajı yazdırma
        console.log("Merhaba Dünya!");
        
        // Değişken değer yazdırma
        let x = 10;
        let y = 20;
        let topla = x + y;
        console.log(topla); // Çıktı: 30
    </script>
    
    <p>Not: Klavyedeki F12 tuşuna basarak tarayıcı konsoluna (console) bakın.</p>

</body>
</html>
```

#### Bir Uyarıyı İletişim Kutusuna Yazma

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Bir Uyarıyı İletişim Kutusuna Yazma</title>
</head>
<body>

    <script>
        // Basit bir kısa mesaj görüntüleme
        alert("Merhaba Dünya!");
        
        // Değişken değer görüntüleme
        let x = 10;
        let y = 20;
        let topla = x + y;
        alert(topla); // Çıktı: 30
    </script>

</body>
</html>
```

#### Tarayıcı Penceresine Yazma

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>Tarayıcı Penceresine Yazma</title>
</head>
<body>

    <script>
        // Basit bir kısa mesaj yazdırma
        document.write("Merhaba Dünya!");
        
        // Değişken değer yazdırma
        let x = 10;
        let y = 20;
        let topla = x + y;
        document.write(topla); // Çıktı: 30
    </script>

</body>
</html>
```

#### document.write() Yöntemle İlgili Sorun

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>document.write() Yöntemle İlgili Sorun</title>
</head>
<body>
    
    <h1>Bu bir başlık</h1>
    <p>Bu bir paragraf metindir.</p>
    
    <button type="button" onclick="document.write('Merhaba Dünya!')">Tıkla</button>

</body>
</html>
```

#### HTML Öğesine Yazdırma

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>HTML Öğesine Yazdırma</title>
</head>
<body>

    <p id="harika"></p>
    <p id="sonuc"></p>
    
    <script>
        // Bir öğenin içine metin dizesi yazma
        document.getElementById("harika").innerHTML = "Merhaba Dünya!";
        
        // Bir öğenin içine değişken bir değer yazma
        let x = 10;
        let y = 20;
        let topla = x + y;
        document.getElementById("sonuc").innerHTML = topla;
    </script>

</body>
</html>
```

#### JavaScript'te Gerçek API ile Bağlantı Kurma ve Veri Çekme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript'te Gerçek API ile Bağlantı Kurma ve Veri Çekme</title>
</head>
<body>

    <script>
        const yazilar = fetch("https://api.dailysmarty.com/posts");
        // console.log(yazilar);

        yazilar
        .then(data => data.json())
        .then(data => {
            data.posts.forEach((item) => {      
            document.write("<a href='" + item.url_for_post + "'>" + item.title + "</a><br>");
            });
        })
        
        .catch((err) => {
            console.log(err);
        })
    </script>

</body>
</html>
```

#### JavaScript'te Attribute Kullanarak Öznitelikleri Değiştirme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript'te Attribute Kullanarak Öznitelikleri Değiştirme</title>
</head>
<body>

    <a href="https://www.pexels.com" target="_blank">Pexel.com</a>

    <hr>

    <img src="https://images.pexels.com/photos/4207892/pexels-photo-4207892.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" width="50%">

    <img src="https://images.pexels.com/photos/2868871/pexels-photo-2868871.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" width="50%">

    <script>
        // Bağlantı linkini değiştirme
        let a = document.querySelector("a");
        console.log(a);
        a.setAttribute("href", "https://www.unsplash.com");
        
        // Birinci görseli bulup yeni resimle değiştirme
        let img1 = document.querySelectorAll("img")[0];
        console.log(img1);
        img1.setAttribute("src", "https://images.pexels.com/photos/4048182/pexels-photo-4048182.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500");

        // İkinci görseli bulup yeni resimle değiştirme
        let img2 = document.querySelectorAll("img")[1];
        console.log(img2);
        img2.setAttribute("src", "https://images.pexels.com/photos/4171211/pexels-photo-4171211.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500");
    </script>

</body>
</html>
```

#### JavaScript'te Click Event Kullanarak Kutuları Gizleme

```
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <title>JavaScript'te Click Event Kullanarak Kutuları Gizleme</title>
    <style>
        .kutu{
            width: 150px;
            height: 150px;
            margin: 10px;
            float: left;
        }

        #mavi{
            background-color: blue;
        }
        #kirmizi{
            background-color: red;
        }
        #sari{
            background-color: yellow;
        }
    </style>
</head>
<body>

    <div id="mavi" class="kutu"></div>
    <div id="kirmizi" class="kutu"></div>
    <div id="sari" class="kutu"></div>

    <script>

        let kutular = document.querySelectorAll(".kutu");

        kutular.forEach(function(kutu){                
            kutu.addEventListener("click", function(){
                this.style.display = "none";
            })
        });

    </script>

</body>
</html>
```