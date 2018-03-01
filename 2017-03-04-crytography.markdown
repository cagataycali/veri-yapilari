---
layout: post
title: "Kriptoli Nedir? Bazı Şifreleme Teknikleri"
excerpt: "Kriptolojiye Giriş...<br>Kriptoloji: En temel anlamda şifre bilimidir. Kriptografi ve Kriptoanaliz gibi konuları işleyen daldır.</br>"
date: 2017-03-04 15:25:00
comments: true
categories: [Kriptoloji]
tags: [Kriptoloji]
---
**`Kriptoloji:`** En temel anlamda şifre bilimidir. Kriptografi ve Kriptoanaliz gibi konuları işleyen daldır.

**`Kriptografi:`** Verileri gizliliği, kimlik denetimi, bütünlüğü gibi bilgi güvenliği kavramlarını sağlamak için oluşturulmuş **<font color="000066">matematiksel</font>** yöntemler bütünüdür. Kriptografi verilerin üçüncü şahısların okumasını engelleyen protokoller ile oluşturulması ve oluşturulmuş olan protokollerin analiz edilmesi ile de ilgilenir.

**`Kriptoanaliz:`** Bir şifreleme şemasında oluşmuş güçsüzlükleri veya güvensizlikleri bulmak ile ilgilenir.

**`Encryption:`** Kriptografi de bir mesajın veya bilginin sadece yetkili kişiler tarafından erişebileceği şekilde kodlanması işlemidir.

**`Decryption:`** Kriptografi de şifrelenmiş bir metin veya verinin alınıp, gönderilen kişinin veya bilgisayarın okuyabileceği şekillere dönüştürme işlemidir.

<h4><b>KRİPTOLOJİNİN KÖKENİ (ORİGİN OF CRYPTOLOGY)</b></h4>

Kriptolojinin sandığımız gibi yakın bir geçmişi yoktur.

 * Kriptolojinin ilk örneğine Roma ve Mısır Uygarlıklarında rastlanır. MÖ 4000 yıllarında Antik Mısırlılar, Hiyerogrif yazıtlarında bazı şifrelemeler yapmışlardır. Bu şifrelemeler daha önce hiç kullanılmamıştır.

* MÖ 5.yy'lar da _"Julius Caesar"_ şimdilerde _Sezar Şifrelemesi_ olarak bilinen bir yöntem geliştirdi. Bu yöntem basit anlamda harlerin 3 harf atlamalı olarak harflerin alfabedeki sırasından 3 harf sonraki harf gelmesi ile oluşturulur. Bu konuyla ilgili ayrıntılı açıklamayı aşağıda bulabilirsiniz.

  Bu dönemde askeri istihbaratta gerekli olan gizlilik sebepleri nedeniyle kriptografi askeri alana girmiştir. Askeri alanda ilk kriptograflar Spartalılardır.
* MÖ 1.yy'lara geldiğimizde Gaznelilerden günümüze kalmış bazı dökümanlarda şifreli metinlere rastlanmıştır. Bir tarihçiye göre dönemdeki yüksek makamlı devlet görevlilerin yeni görev yerlerine giderken şahsa özel şifreleme bilgileri veriliyordu.

* 1585 yılında _"Blaise de Vigenére"_ kriptoloji üzerine bir kitap yazdı. İlk kez bu kitapta şifreli metin için otomatik anahtarlama yönteminden bahsedildi. Günümüzde bu yöntem hala DES, CBC ve CFB kiplerinde kullanılmaktadır.

* 1963 yılında _"Sir Francis Bacon"_, 5-bitlik ikili kodlamayla karakter tipi değişikliğine dayanan _Steganografi_ yöntemini buldu. Steganografi temel anlamda "gizlenmiş yazı" anlamına gelir ve bilgiyi gizleme bilimine verilen addır.

* 20.yy'da II. Dünya Savaşı'nda _"William Frederick Friedman"_, _"Riverbank Laboratuvarları"_'nı kurdu ve ABD için kriptoanaliz çalışmaları yaptı. Japonlar'ın _Purple Machine_ şifrelemesini çözdü.

  Yine II.Dünya Savaşı sırasında _"Alman Arthur Scherbius"_ tarafından icat edilmiş _"Enigma"_ makinasını _"Alan Turing"_ ve ekibi çözmüştür.
* 1970'lerde _Horst Feistel (IBM)_ DES'in temelini oluşturan _"Lucifer Algoritması"_'nı geliştirdi.

* 1978 yılında _Ronald Rivest_, _Adi Shamir_ ve _Leonard Adleman_ RSA Algoritmasını geliştirdiler.

* 1990 yılında _Xuejia Lai_ ve _James Massey_; IDEA Algoritmasını geliştirdi.

<h3><b>ŞİFRELEME TEKNİKLERİ</b></h3>

  ***SEZAR ŞİFRELEMESİ (CAESAR CIPHER)***

Bu şifrelemede var olan metindeki her harf için alfabedeki sırasından 3 harf sonraki harf gelerek oluşturulmuş bir şifreleme yöntemidir.

<img src="{{ site.url }}/img/kgiris/sezar.jpg" alt="{{ site.title }}">

> Plain   :ABCDEFGHIJKLMNOPQRSTUVWXYZ
>
> Cipher  :XYZABCDEFGHIJKLMNOPQRSTUVW

>Plain    :R E M Z I D A L Y A N
>
>Cipher   :U H P C L G E O B D Q

  ***VİGENÉRE ŞİFRELEMESİ (VIGENÉRE CIPHER)***

Alfabetik mantığı (sezar şifrelemesi ile benzer bir mantık) kullanılarak oluşturulmuş bir şifreleme yöntemidir. Blaise de Vigenére tarafından oluşturulmuştur.

<img src="{{ site.url }}/img/kgiris/vigenere.jpg" alt="{{ site.title }}">

> Plaintext   : A T T A C K A T D A W N
>
> Key         : L E M O N L E M O N L E
>
> Ciphertext  : L X F O P V E F R N H R

Plain text bizim şifrelemek istediğimiz mesajımız onun için yataydaki harfleri kullanacağız. Key bizim şifreyebilmek için kullanacağımız anahtarımız onun içinde dikey harfleri kullanacağız. Plaintext A harfi ile keydeki L harfinin kesişim noktasında L harfi bulunuyor. Plaintext T harfi ile keydeki E harfinin kesişim noktasında X harfi bulunuyor. Bu şekilde devam ediyor. Biz metni şifreliyoruz.

  ***STEGANOGRAFİ***

Gizlenmiş yazı anlamına gelir ve bilgiyi gizleme bilimine verilen addır. Bu konunun şifrelemeden en önemli farkı gördüğün şeyin içinde önemli bir bilginin gizli olduğunun bilinmemesi veya farkında olunmamasıdır.

<img src="{{ site.url }}/img/kgiris/steganografi.jpg" alt="{{ site.title }}">

***Bilgisayar Dünyasında Kuallanımı***

En önemli örneği veri içine veri gömmektir. Resim, ses veya müzik gibi büyük boyutlu dosyaların kodları içine periyodik olarak yapılan bozukluğu insan kulağı veya gözü algıyamaz.

<img src="{{ site.url }}/img/kgiris/steganografi2.jpg" alt="{{ site.title }}">

  ***ÖZET FONKSİYONLARI (HASH FUNCTION)***

Özet fonksiyonları değişken veri kümelerini, sabit uzunluklu veri kümelerine düzenleyen algoritmadır. <font color="red">Örneğin:</font> Değişken uzunluktaki isimleri, tekil tam sayılar olarak hashlenebilir.

Anlaşılması en basit özet fonsiyonu modülo işlemidir. Buna göre mod10 işlemini ele alalım aşağıdaki sayıları listeleyelim.
> **Sayılar:** 10 - 8 - 36 - 42 - 64 - 58 - 78 - 65 - 2356 - 7984 - 4123 - 1565 - 262 - 131 - 81 - 79

<img src="{{ site.url }}/img/kgiris/hash2.jpg" alt="{{ site.title }}">

Yukarıdaki sayıları tek haneli sayılara özetlenmiştir. Tabi ki aynı sayıya özetlenen sayılar olabilir bu durumda çakışma olur.

özet fonksiyonları, veritabanında tabloda aranan veriyi hızlı bir şekilde bulmak, veri karşılaştırması işlemlerini hızlandırmak, büyük bir dosyada benzer kayıtları tespit etmek, DNA dizisinde benzer dizilimleri bulmak gibi işlemler için kullanılır.

<img src="{{ site.url }}/img/kgiris/hash.jpg" alt="{{ site.title }}">

> Resimde görüldüğü gibi çakışma söz konusu olduğunda aynı anahtara ait veriler çakışabilir. Veriler çakıştıkları bu noktadan itibaren bağlı liste olarak dallanır. Örneğin:   2 Anahtarına ait 2 farklı veri geldi bu veriler 2 anahtarından itibaren bağlı liste kuracaktır.
