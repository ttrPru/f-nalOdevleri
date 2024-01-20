Uçak Bilet Rezervasyon Uygulaması

Bu basit uçak bilet rezervasyon uygulaması, C# programlama dilinde nesneye dayalı programlama (OOP) prensiplerini kullanarak geliştirilmiştir. Uygulama, uçak, lokasyon, uçuş ve rezervasyon işlemlerini yönetmek için dört temel sınıf içerir. Ayrıca, kaydedilen bilgileri JSON formatında dosyalara yazma ve okuma işlemlerini gerçekleştirebilen bir uygulama sınıfı içerir.

Sınıflar ve Özellikleri
Ucak Sınıfı

Model: Uçağın modelini temsil eder.
Marka: Uçağın markasını temsil eder.
SeriNo: Uçağın seri numarasını temsil eder.
KoltukKapasitesi: Uçağın koltuk kapasitesini temsil eder.
Lokasyon Sınıfı

Ulke: Lokasyonun bulunduğu ülkeyi temsil eder.
Sehir: Lokasyonun bulunduğu şehiri temsil eder.
Havaalani: Lokasyonun havaalanını temsil eder.
Aktif: Lokasyonun aktif olup olmadığını temsil eder.
Ucus Sınıfı

KalkisYeri: Uçuşun kalkış yerini temsil eder (Lokasyon tipinde).
VarisYeri: Uçuşun varış yerini temsil eder (Lokasyon tipinde).
Saat: Uçuşun gerçekleşeceği saat ve tarihi temsil eder.
UcakBilgisi: Uçuşun kullanacağı uçağı temsil eder (Ucak tipinde).
Rezervasyon Sınıfı

UcusBilgisi: Rezervasyonun yapıldığı uçuş bilgisini temsil eder (Ucus tipinde).
Ad: Rezervasyonu yapan kişinin adını temsil eder.
Soyad: Rezervasyonu yapan kişinin soyadını temsil eder.
Yas: Rezervasyonu yapan kişinin yaşını temsil eder.
Uygulama Sınıfı

Ucaklar: Uygulamadaki uçakları içeren liste.
Lokasyonlar: Uygulamadaki lokasyonları içeren liste.
Ucuslar: Uygulamadaki uçuşları içeren liste.
Rezervasyonlar: Uygulamadaki rezervasyonları içeren liste.
Temel İşlemler
Uçak Ekleme

UcakEkle metodu ile uygulamaya yeni bir uçak ekleyebilirsiniz.
Lokasyon Ekleme

LokasyonEkle metodu ile uygulamaya yeni bir lokasyon ekleyebilirsiniz.
Uçuş Ekleme

UcusEkle metodu ile uygulamaya yeni bir uçuş ekleyebilirsiniz.
Rezervasyon Yapma

RezervasyonYap metodu ile uygulama üzerinden rezervasyon yapabilirsiniz. Rezervasyon yapılırken uçuşun ve uçağın durumları kontrol edilir.
Tüm Bilgileri Kaydetme

TumBilgileriKaydet metodu ile uygulamadaki tüm bilgileri JSON formatında bir dosyaya kaydedebilirsiniz.
Tüm Bilgileri Yükleme

TumBilgileriYukle metodu ile önceden kaydedilmiş tüm bilgileri JSON dosyasından yükleyebilirsiniz.
Uygulama Kullanımı
Uygulama, Uygulama sınıfındaki Main metodunda örnek bir senaryo ile kullanılmıştır. Bu senaryoda uçak, lokasyon, uçuş ve rezervasyon işlemleri gerçekleştirilmiş, tüm bilgiler JSON dosyasına kaydedilmiş ve ardından bu bilgiler tekrar yüklenmiştir. Bu örnek senaryo, uygulamanın temel fonksiyonlarını anlamanıza yardımcı olabilir. Dilerseniz kendi senaryolarınıza göre uygulamayı kullanabilirsiniz.

Bağımlılıklar
Json.NET (Newtonsoft.Json) - JSON işlemleri için kullanılmıştır.
