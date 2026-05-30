# Adam-Asmaca-Oyunu
Java Swing ile geliştirilmiş şifre kontrollü Adam Asmaca oyunu.
# Adam Asmaca Oyunu

Bu proje, Java Swing kullanılarak geliştirilmiş bir **Adam Asmaca** oyunudur. Proje Apache NetBeans ortamında hazırlanmıştır. Oyunda kullanıcı şifre kontrolünden geçtikten sonra rastgele seçilen kelimeyi harf veya kelime tahmini yaparak bulmaya çalışır.

## Projenin Amacı

Bu projenin amacı; Java programlama dili kullanılarak dosya işlemleri, Swing arayüz tasarımı, JTable, JTabbedPane, JMenuBar, Timer ve temel oyun mantığının birlikte kullanıldığı bir masaüstü uygulaması geliştirmektir.

## Kullanılan Teknolojiler

* Java
* Java Swing
* Apache NetBeans
* JFrame
* JPanel
* JLabel
* JTextField
* JButton
* JTable
* JTabbedPane
* JMenuBar
* Timer
* Dosya işlemleri

## Oyun Özellikleri

* Program açıldığında şifre kontrolü yapılır.
* Eğer daha önce şifre oluşturulmamışsa kullanıcıdan alınan şifre `sifre.txt` dosyasına kaydedilir.
* Daha önce şifre belirlenmişse girilen şifre dosyadaki şifre ile karşılaştırılır.
* Kullanıcı 3 kez yanlış şifre girerse program kapanır.
* Her şifre denemesi tarih ve saat bilgisi ile birlikte `log.txt` dosyasına kaydedilir.
* Oyun ekranında `JTabbedPane` kullanılmıştır.
* Oyunda üç sekme bulunmaktadır:

  * Oyun Oynama
  * Eski Skorlar
  * Loglar
* Oyun başladığında `kelimeler.txt` dosyasından rastgele bir kelime seçilir.
* Seçilen kelime ekranda yıldız karakterleri ile gösterilir.
* Kullanıcı harf tahmini yapabilir.
* Kullanıcı kelime tahmini yapabilir.
* Yanlış tahminlerde adam asmaca resmi adım adım değişir.
* Kullanıcı 11 yanlış tahmin yaparsa oyun kaybedilir.
* Oyun sırasında süre saniye olarak tutulur.
* Oyun kazanılsa da kaybedilse de sonuç `oyunlar.txt` dosyasına kaydedilir.
* Eski oyun skorları JTable ile görüntülenebilir.
* Log kayıtları JTable ile görüntülenebilir.
* Skorlar ve loglar şifre kontrolü ile temizlenebilir.
* Menü çubuğu kullanılarak oyuna başlama ve oyunu yeniden başlatma işlemleri yapılabilir.

## Dosya Yapısı

Projenin çalışması için dosyalar aşağıdaki klasör yapısında bulunmalıdır:

```text
C:\P2Oyun
│
├── Resimler
│   ├── 1.jpg
│   ├── 2.jpg
│   ├── 3.jpg
│   ├── 4.jpg
│   ├── 5.jpg
│   ├── 6.jpg
│   ├── 7.jpg
│   ├── 8.jpg
│   ├── 9.jpg
│   ├── 10.jpg
│   └── 11.jpg
│
└── TXTDosyalar
    ├── kelimeler.txt
    ├── sifre.txt
    ├── log.txt
    └── oyunlar.txt
```

## TXT Dosyalarının Görevleri

### kelimeler.txt

Oyunda rastgele seçilecek kelimeler bu dosyada tutulur. Dosyada en az 6 harften oluşan 30 kelime bulunmaktadır.

### sifre.txt

Kullanıcının giriş şifresi bu dosyada saklanır. Eğer dosya boşsa ilk girişte şifre oluşturulur.

### log.txt

Kullanıcının şifre denemeleri ve giriş işlemleri tarih-saat bilgisiyle bu dosyaya yazılır.

### oyunlar.txt

Oyun sonunda kullanıcının kazanıp kazanmadığı, oyun süresi ve tarih-saat bilgisi bu dosyaya kaydedilir.

## Oyun Ekranı

Oyun ekranında kullanıcıya yıldızlarla gizlenmiş bir kelime gösterilir. Kullanıcı harf tahmini veya kelime tahmini yaparak kelimeyi bulmaya çalışır.

Yanlış tahmin yapıldığında adam asmaca görseli bir sonraki aşamaya geçer. Toplam 11 yanlış tahmin hakkı vardır.

## Eski Skorlar Ekranı

Bu sekmede daha önce oynanan oyunların sonuçları JTable üzerinde listelenir. Kullanıcı oyun süresini, sonucu ve oynama tarihini görebilir.

Ayrıca “Temizle” butonu ile şifre doğrulaması yapıldıktan sonra eski skor kayıtları silinebilir.

## Loglar Ekranı

Bu sekmede kullanıcı girişleri ve şifre denemeleri JTable ile görüntülenir.

“Temizle” butonu ile şifre doğrulaması yapıldıktan sonra log kayıtları temizlenebilir.

## Menü Yapısı

Projede JMenuBar kullanılmıştır. Menü üzerinden oyuna başlama ve oyunu yeniden başlatma işlemleri yapılabilir.

## Kurulum ve Çalıştırma

1. `P2Oyun` klasörü C diskine yerleştirilmelidir.
2. `Resimler` klasörü içinde 1.jpg ile 11.jpg arasındaki görseller bulunmalıdır.
3. `TXTDosyalar` klasörü içinde gerekli txt dosyaları bulunmalıdır.
4. Proje Apache NetBeans ile açılmalıdır.
5. Proje çalıştırıldığında önce şifre ekranı açılır.
6. Doğru şifre girildiğinde oyun ekranına geçilir.

## Proje Geliştirme Süreci

Proje geliştirilirken önce dosya yapısı oluşturulmuştur. Daha sonra şifre kontrol ekranı hazırlanmıştır. Şifre sistemi tamamlandıktan sonra oyun ekranı tasarlanmıştır. Oyun ekranında sekmeli yapı kullanılmış ve oyun oynama, eski skorlar ve loglar bölümleri ayrı ayrı hazırlanmıştır.

Daha sonra harf tahmini, kelime tahmini, süre sayacı, resimlerin değişmesi, oyun sonucunun kaydedilmesi ve kayıtların JTable üzerinde görüntülenmesi özellikleri eklenmiştir.

## Sonuç

Bu proje ile Java Swing kullanılarak dosya işlemleriyle çalışan, şifre kontrollü, görsel arayüze sahip bir Adam Asmaca oyunu geliştirilmiştir. Projede temel Java bilgileri, Swing bileşenleri ve dosya okuma-yazma işlemleri birlikte kullanılmıştır.
