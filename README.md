#Oto Yıkama Müşteri Takibi Web Uygulaması

DÖKÜMAN

İsmayil Öztürk Ögr No: 132130122 Bursa Uludağ Üniversitesi

**Bu web uygulaması kime hitap ediyor?**
<br>
Oto Yıkama işletmelerine hitap etmektedir.

**Hangi problemi çözüyor?**
<br>
Yoğun anlarda, araç sahiplerinin ve hizmetin karışmasını çözmektedir.

**Nasıl ve hangi senaryoda kullanılıyor?**
<br>
Müşteri işletmeye geldiğinde iletişim bilgileri, plaka, hizmet türü ve tarih bilgisi sisteme girilmektedir. Yoğunluk gerçekleştiği zamanlarda kullanılmaktadır.

**Kullanılan Teknolojiler**
<br>
C#, ASP.NET MVC, SQL SERVER EXPRESS

**Youtube Link**
<br><br>
Link: https://youtu.be/1ZHsfyYb2Zo

Özellikler
+Müşteri Bilgisi Listeleme
+Müşteri Bilgisi Ekleme
+Müşteri Bilgisi Görüntüleme (Detay)
+Müşteri Bilgisi Düzenleme
+Müşteri Bilgisi Silme

Listelenen bilgiler:
<br>
Ad Soyad - Telefon - Plaka - Hizmet Adı - Hizmet Tarihi
<br><br>

Müşteri Bilgisi Listeleme (Index.cshtml)
<img width="1562" height="534" alt="index" src="https://github.com/user-attachments/assets/45ed1d55-d9be-4bdf-a177-5064352f531a" />

Müşteri Bilgisi Ekleme (Yeni.cshtml)
<img width="1593" height="598" alt="create" src="https://github.com/user-attachments/assets/ecb0e6f9-aeba-48fb-b548-92b2421b1912" />

Müşteri Bilgisi Görüntüleme (Detay.cshtml)
<img width="1581" height="541" alt="read" src="https://github.com/user-attachments/assets/a5534d05-bf73-43cd-9c15-65a78c322fa7" />

Müşteri Bilgisi Düzenleme (Duzenle.cshtml)
<img width="1608" height="779" alt="edit" src="https://github.com/user-attachments/assets/9b7b36d1-9ed0-4ece-96c3-464b732cbac9" />

Müşteri Bilgisi Silme (Sil.cshtml)
<img width="1576" height="615" alt="delete" src="https://github.com/user-attachments/assets/0c5fbbd2-9b6a-47e6-96a8-fcf1fcf12605" />

Veritabanı Tablo ve Sütun Yapısı için SQL Kodları:

CREATE DATABASE OtoYikamaVeritabani;

USE OtoYikamaVeritabani;
CREATE TABLE Musteriler (
Id INT PRIMARY KEY IDENTITY(1,1),
AdSoyad NVARCHAR(100) NOT NULL,
Telefon NVARCHAR(15) NOT NULL,
Plaka NVARCHAR(15) NOT NULL,
Hizmet NVARCHAR (15) NOT NULL,
HizmetTarihi DATETIME
);
