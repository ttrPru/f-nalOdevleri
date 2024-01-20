Uygulama - Öğrenci ve Ders Bilgi Sistemi
Bu Java uygulaması, öğrenci, ders ve öğretim görevlisi bilgilerini yönetmek için bir sistem sunar. Sistem, bu bilgileri dosyaya kaydedebilir ve dosyadan yükleyebilir. Ayrıca, örnek veri ekleyerek uygulamanın temel işlevselliğini test edebilirsiniz.

Ders Sınıfı
Ders sınıfı, bir dersin temel bilgilerini depolamak için kullanılır.
dersKodu: Dersin kodunu temsil eder.
dersAd: Dersin adını temsil eder.
dersDonem: Dersin hangi dönemde okutulduğunu belirtir.
ogretimGorevlisi: Dersi öğreten öğretim görevlisinin adını içerir.
toString(): Ders sınıfının örneğini düz metin formatında temsil eder.

Ogrenci Sınıfı
Ogrenci sınıfı, bir öğrencinin bilgilerini depolamak için kullanılır.
ogrenciNo: Öğrenci numarasını temsil eder.
ogrenciAd: Öğrencinin adını temsil eder.
ogrenciSoyad: Öğrencinin soyadını temsil eder.
ogrenciBolum: Öğrencinin kayıtlı olduğu bölümü temsil eder.
ogrenciDersler: Öğrencinin aldığı dersleri içeren bir liste.
toString(): Ogrenci sınıfının örneğini düz metin formatında temsil eder.

OgretimGorevlisi Sınıfı
OgretimGorevlisi sınıfı, bir öğretim görevlisinin bilgilerini depolamak için kullanılır.
ogretmenNo: Öğretim görevlisinin numarasını temsil eder.
ad: Öğretim görevlisinin adını temsil eder.
soyad: Öğretim görevlisinin soyadını temsil eder.
bolum: Öğretim görevlisinin çalıştığı bölümü temsil eder.
verdigiDersler: Öğretim görevlisinin verdiği dersleri içeren bir liste.
toString(): OgretimGorevlisi sınıfının örneğini düz metin formatında temsil eder.

Uygulama Sınıfı
Uygulama sınıfı, ana uygulama mantığını içerir.
dersListesi, ogrenciListesi ve ogretimGorevlisiListesi: Ders, öğrenci ve öğretim görevlisi bilgilerini içeren listeler.
testVerileriEkle(): Uygulamanın temel işlevselliğini test etmek için örnek verileri ekler.
tumBilgileriKaydet(String dosyaAdi): Tüm bilgileri belirtilen dosyaya kaydeder.
tumBilgileriYukle(String dosyaAdi): Belirtilen dosyadan tüm bilgileri yükler.

Kullanım
Uygulama sınıfındaki main metodu çalıştırarak uygulamayı başlatın.
testVerileriEkle() metodu ile örnek verileri ekleyin.
tumBilgileriKaydet() ve tumBilgileriYukle() metotlarıyla bilgileri dosyaya kaydedin ve dosyadan yükleyin.

Notlar
Uygulama, Serializable arabirimini kullanarak nesnelerin serileştirilmesini ve deserializasyonunu gerçekleştirir.
Tüm bilgiler, JSON formatında bir dosyaya kaydedilir ve bu dosya üzerinden yüklenir.
Örneğin, "tumBilgiler.json" adlı bir dosya kullanılmaktadır.
Bu README dosyası, uygulamanın temel özelliklerini ve kullanımını özetlemektedir. Daha fazla bilgi için kodları inceleyebilir ve detaylı anlamak için yorum satırlarına başvurabilirsiniz.
