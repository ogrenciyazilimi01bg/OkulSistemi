#OkulSistemi
##Genel bakış
Bu projede, Okul Sistemi için geliştirilen kodların kaynağı yer almaktadır. Bu proje, Java dilinde yazılmış bir  Okul sistemi uygulamasını içermektedir.Proje temelde Okul  Uygulaması niteliğinde Windows Form üzerinden
yapılmaktadır. Proje kullanıcının istekleri doğrultusunda Ögrenci kaydı,Ogrenci kayıtlarını listeleme ,Öğretim görevlisi bilgileri kaydı,Öğretim bilgisi verileri listeleme ,ders kaydı yapma ve ders kaydı listeleme
yapmayı amaçlamaktadır. Bu yönergeleri, projeyi kendi makinenizde çalıştırmak ve geliştirmek için kullanabilirsiniz. ###Temel Bileşenler DersKayit sınıfı içinde ders adı, derskodu, dersdonemi, ogretimgörevlisi ve
dersbolum gibi özelliklere sahiptir. Bu sınıf, ders bilgilerini yönetmek ve erişmek için get ve set metotlarını içerir. OgrenciKayit sınıfı, öğrenci bilgilerini temsil eder. Oğrenciadı, Ogrencisoyadı, Ogrencino,
Ogrencibolum,Ogrencidonem, Ogrenciderssecimi gibi bilgiler bu sınıf üzerinden yönetilir. Ogretimgorevlisi sınıfı,ogretim gorevlisi bilgilerini temsil eder. OgretimgorevlisiAdi, OgretimGorevlisisoyadi, 
OgretimGorevlisiNo, OgretimGorevlisibolum, gibi bilgiler bu sınıf üzerinden yönetilir. ###Kullanıcı Arayüzü Menu sınıfı, ana menüyü temsil eder ve kullanıcıya "Ders  Formu","Ogretim Gorevlisi  Formu"  ve "Öğrenci 
Formu" seçeneklerini sunar. Kullanıcı, menü üzerinden istediği formu seçerek işlemlerine devam edebilir. DersFormu sınıfı, kullanıcıya ders kayıtlarını girebileceği bir arayüz sunar. Kullanıcı, dersin adı,ders kodu,
dersdönemi, dershocası ve verilecek ders bölümü gibi bilgileri girerek yeni ders kaydı ekleyebilir. Burdan Dersler ile ilgili kayıtları görebilir.Burdan filtreleyerekte verileri inceleyebilir kullanıcı. 
ogretimGorevlisiFormu sınıfı, kullanıcıya öğretim görevlisi kayıtlarını girebileceği bir arayüz sunar. Kullanıcı, Ogretim görevlisiadı,OgretimgörevlisiSoyadi,ogretimGorevlisiNo,  ve verilecek ogretimGorevlisiBolum
gibi bilgileri girerek yeni öğretim görevlisi kaydı ekleyebilir. Burdan Ogretim Görevlisi ile ilgili kayıtları görebilir.Burdan filtreleyerekte verileri inceleyebilir kullanıcı. Ve OgrenciFormu sınıfı, öğrenci 
bilgilerini girebilmek için tasarlanmış arayüzü içerir. Kullanıcı, öğrencinin adı, soyadı, numarası, bölümü, dönemi, ders seçimi ve gibi bilgileri girebilir.Bunlardan Bölümü ,dönemi ve ders seçimi combobox tarzı
yapıldı. Burdan Ogrenci ile ilgili kayıtları görebilir.Burdan filtreleyerekte verileri inceleyebilir kullanıcı. ###Dosya İşlemleri Uygulama, kayıtları dosyalarda saklar ve dosyadan okuma/yazma işlemleri gerçekleştirir.
Kaydedilen veri dosyası dersKayit.csv,ogretimGorevlisi.csv ve ogrenci.csv adlarını taşır.
## Uygulama şu şekilde çalışır:
Uygulama intellij idea uygulamasında çalıştırılır.Kullanıcı menüden 3 seçenekten birini seçer . Ders  Formu butonunu seçerse ders kaydı yapar burda istenilen veriler girilir.Ders Adı,Ders Kodu,Ders Dönemi,
Verilecek DersBölümü ve OgretimGorevlisi verileri girilir .Verilecek ders bölüm ,ogretim görevlisi ve donem comboboxtan seçilir.Comboboxta seçilen bolume göre öğretim goörevlisi isimleri ogretim goörevlis alanında
combobox’ta çıkar.Ders Kaydet butonuna basılır.Ders bilgileri kaydedilir.Burdan filtreleme yaparak istediği Ders kayıtları ile ilgili bilgileri inceleyebilir yada tüm verileri listeleyebilir.Arama yerine”donem” yazarsa
donem bilgileri,”dersKodu” yazarsa ders kodu bilgileri,”bölüm” yazarsa bölüm bilgileri,”ogretim görevlisi” yazarsa öğretim görevlisi verileri ,“ders adı” yazarsa ders adı verileri yada boş bırakıp enter tuşuna basar 
ararsa tüm kayıtlar çıkar ders ile ilgili. Öğrenci formu butonuna basılırsa ogrenci  formu sayfası açılır.Öğrenci bilgilerinin burda eksiksiz girilmesi istenir.Öğrenci Adı,Öğrenci soyadı,Öğrenci No ve diğer bilgiler 
girilir. Öğrenci combobox'tan bölümünü seçer .Seçilen bölüme göre var olan o dönemler bölüme göre dönem bilgisi çıkar dönem combobox'ta .Bu çıkan dönem bilgisinden de dönem seçilince o bölümün o dönemine ait dersler ,
dersler combobox'ında gözükür.Ordanda ders seçilir .Ardından öğrenci kaydet butonuna basarak öğrenci kaydedilir..Burdan filtreleme yaparak istediği Öğrenci kayıtları ile ilgili bilgileri inceleyebilir yada tüm verileri
listeleyebilir.Arama yerine”ad” yazarsa ad bilgileri,”soyad” yazarsa soyad  bilgileri,”bolum” yazarsa bölüm bilgileri,”ogrenci no” yazarsa öğrenci no verileri ,“alınan ders ” yazarsa alınan ders adı verileri,”donem”
yazarsa donem bilgileri yada boş bırakıp enter tuşuna basar ararsa tüm kayıtlar listelenir .OgretimGorevlisi formu butonuna basılırsa ogretim gorevlisi  formu sayfası açılır.Öğretim görevlisi bilgilerinin burda eksiksiz 
girilmesi istenir.ÖğretimGörevlisi Adı,ÖğretimGörevlisi soyadı,ÖğretimGorevlisiNo ve diğer bilgiler girilir. Öğretim görevlisi combobox'tan bölümünü seçer . Ardından öğretim görevlisiBilgileri kaydet butonuna basarak
öğretimgörevlisi kaydedilir.Burdan filtreleme yaparak istediği Öğretim görevlisi kayıtları ile ilgili bilgileri inceleyebilir yada tüm verileri listeleyebilir.Arama yerine”ad” yazarsa ad bilgileri,”soyad” yazarsa soyad 
bilgileri,”bolum” yazarsa bölüm bilgileri,”ogretim görevlisi no” yazarsa öğretimgörevlisi no verileri yada boş bırakıp enter tuşuna basar ararsa tüm kayıtlar listelenir .Bu üç form sayfasında menu butonu var.Bu butona 
basarak menü sayfasına dönülebilir.

