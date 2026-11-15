# LANDesk

LANDesk ile aynı yerel ağdaki Windows bilgisayarların ekranını görüntüleyebilir, fare ve klavye ile kontrol edebilirsiniz. Ana bilgisayarda ve kontrol edilecek bilgisayarlarda aynı uygulamayı kullanırsınız.

[Windows x64 paketini indir](https://github.com/alikocidev/LANDesk-releases/releases/latest/download/LANDesk-Windows.zip) · [Sürümler](https://github.com/alikocidev/LANDesk-releases/releases)

## Gereksinimler

- Windows x64.
- Bilgisayarlar arasında aynı yerel ağ bağlantısı. Wi-Fi ve Ethernet birlikte kullanılabilir.
- Kontrol edilecek bilgisayarda açık, kilitsiz bir Windows oturumu ve çalışan LANDesk.

Güncelleme indirmek için internet bağlantısı gerekir.

## Kurulum

1. ZIP dosyasını indirin ve bir klasöre çıkarın.
2. Her bilgisayarda LANDesk.exe dosyasını açın.
3. Windows Güvenlik Duvarı izin isterse uygulamaya ev ağınızın **Özel ağ** profili için erişim izni verin.

Uygulamayı, güncelleme sırasında dosya yazabileceğiniz bir klasörde tutun.

## Bağlantı kurma

**Ana bilgisayar**, diğer cihazları yönetmek için kullandığınız bilgisayardır. **Hedef bilgisayar**, ekranını ve giriş kontrolünü paylaşan cihazdır.

### Hedef bilgisayarda

1. **Bu bilgisayarı paylaş** düğmesine basın.
2. LANDesk'i açık bırakın. Pencereyi küçültebilirsiniz.

### Ana bilgisayarda

1. **Bilgisayarları bul** düğmesine basın.
2. Hedefi seçip **Seçili bilgisayara bağlan** düğmesine basın.

Kod veya parola istenmez. Paylaşım açıkken aynı yerel ağdaki bilgisayarlar doğrudan bağlanabilir. Paylaşımı durdurmak erişimi keser. LANDesk kayıtlı cihazları hatırlar. Cihaz görünmüyorsa **IP ile ekle** seçeneğini kullanın.

Tüm bilgisayarlarda aynı LANDesk sürümünü kullanın. Sürümler farklıysa bağlantı kurulmaz.

## Fare ve klavye kontrolü

Bağlantı penceresindeki ekran görüntüsüne tıklayın. Fare tıklamaları, sürükleme, kaydırma ve klavye girişleri hedef bilgisayara iletilir.

Varsayılan görüntü hızı 30 FPS'tir. Her bağlantı penceresinin üstündeki **60 FPS** kutusunu işaretleyerek o ekranın hedefini 60 FPS yapabilirsiniz. Seçimi kaldırınca 30 FPS'ye döner. Pencereler ayrı ayarlanır; tercih bilgisayar bazında kaydedilir ve tekrar bağlantıda hatırlanır.

Pencerenin altındaki FPS değeri, saniyede gösterilen gerçek kare sayısını belirtir; seçili hedef ayrıca gösterilir. Ulaşılabilen hız bilgisayarların performansına ve ağ bağlantısına bağlıdır.

- **F12:** Fare ve klavye kontrolünü açar veya kapatır.
- **Bağlantıyı kes:** Açık oturumu kapatır.
- **Paylaşımı durdur:** Hedef bilgisayara erişimi kapatır.

Her hedefe aynı anda bir kontrol oturumu açabilirsiniz. Farklı hedefleri ayrı pencerelerde yönetebilirsiniz. Dört bilgisayara sırayla bağlanıp pencereleri ekranda 2×2 yerleştirebilirsiniz. Fare ve klavye, odaktaki pencereyi kontrol eder.

Listedeki **Bağlantı** sütunu **Bağlı**, **Bağlanıyor…**, **Kapandı** veya **Henüz açılmadı** durumunu gösterir. Açılma bilgisi bu uygulama oturumu için tutulur. Zaten bağlı bir bilgisayarı tekrar açtığınızda mevcut bağlantı penceresi gösterilir.

Görüntü GPU ile çizilir. Tamamen örtülen veya görev çubuğuna küçültülen bağlantı pencerelerinin görüntü yükü otomatik azaltılır; yeniden görünür olduklarında seçili 30/60 FPS hedefi geri gelir. Kısmen görünen pencereler normal hızda kalır. GPU kullanılamıyorsa yazılımsal çizimle devam edilir.

### Knight Online uyarıları

Her bağlantı penceresinin üstündeki **Disconnect izle** ve **Respawn izle** kutuları varsayılan olarak açıktır. Her birini ayrı kapatabilirsiniz; seçimler bilgisayar bazında kaydedilir. Önceki sürümden ilk geçişte kayıtlı bilgisayarlarda da ikisi açılır.

Algılanan uyarı bilgisayar adıyla masaüstünde gösterilir ve ses verir. **Kapat** veya **Ekranı göster** düğmesine basana kadar açık kalır. Aynı uyarı ekranda kaldığı sürece tekrar bildirilmez. Ana listede de son uyarı görünür.

LANDesk penceresi küçültülse de izleme sürer. Hedefte oyun ve uyarı görünür olmalı; tanıma ekranın ortasındaki İngilizce Disconnect/Respawn metinleri içindir. Farklı yazı görünümü veya çok küçük görüntülerde ek ayar gerekebilir.

Uyarı gelmezse diyalog görünürken **Uyarı tanısını kaydet** düğmesini kullanın. Oluşan ZIP, LANDesk tarafından alınan ekran karesini PNG olarak ve son kontrolleri içerir; sorun incelemesinde kullanılabilir. Alt satırdaki **KO** bilgisi izlemenin kontrol durumunu gösterir.

### Telefon bildirimleri (Telegram)

Ana bilgisayardaki **Telefon bildirimleri** düğmesini açın. Bir defalık kurulum:

1. Telegram'da [BotFather](https://t.me/BotFather) üzerinden `/newbot` ile bir bot oluşturun.
2. Bot anahtarını LANDesk'e girip **Eşleştirmeyi başlat** düğmesine basın.
3. Telefondan kendi botunuza ekrandaki kodu mesaj olarak gönderin. **Botu aç** veya **Bağlantıyı kopyala** bağlantısı da aynı eşleştirmeyi başlatabilir.
4. **Telefonu bul**, ardından **Test bildirimi gönder** düğmesine basın.
5. Mesajı telefonda gördüğünüzde **Disconnect ve Respawn uyarılarını Telegram üzerinden gönder** kutusunu işaretleyip **Kaydet** düğmesine basın.

Kayıtlı eşleştirme yeşil **Eşleştirme tamamlandı** durumuyla gösterilir. **Telefonu değiştir** farklı bir hesap için yeni eşleştirme başlatır. Test düğmesi otomatik gönderim kutusundan bağımsız bir deneme mesajı gönderir; otomatik uyarı tercihi Kaydet ile uygulanır. Disconnect ve Respawn, bilgisayar adı ve saatle ayrı Telegram mesajları olarak gönderilir. Mevcut masaüstü uyarıları da devam eder. İzleme tercihini her bağlantı penceresinden ayrı değiştirebilirsiniz.

Telefon bildirimleri için ana bilgisayarda LANDesk ve izlenen bağlantılar açık kalmalıdır. Ana bilgisayar ve telefon internete bağlı olmalıdır; telefon mobil veri kullanabilir. Bot anahtarı Windows kullanıcı hesabına bağlı şifrelenerek yerelde saklanır. Gönderim hatası ana ekrandaki Telegram durumunda görünür.

### Sanal klavye/fare (FakerInput)

Standart giriş yöntemine alternatif olarak FakerInput kullanılabilir. Sürücü yalnızca kontrol edilecek bilgisayara kurulur.

1. Hedefte paylaşım kapalıyken **Sürücüyü kur** düğmesine basın.
2. Windows'un yönetici izin penceresini onaylayın. Standart hesapta yönetici parolası gerekir.
3. **FakerInput hazır** mesajı geldiğinde sanal klavye/fare seçilmiş olur. Paylaşımı açın.
4. Uygulama Windows Installer'ın yeniden başlatma istediğini bildirirse Windows'u yeniden başlatın.

Kurulum paketi EXE'ye dahildir. Sonraki kullanımlarda sürücüyü tekrar kurmanız gerekmez. Giriş yöntemini değiştirmek için önce paylaşımı durdurun; standart yönteme dönmek için **Sanal klavye/fare kullan (FakerInput)** seçimini kaldırın.

FakerInput aynı anda altı normal tuşu ve Shift/Ctrl/Alt/Windows gibi değiştirici tuşları destekler. Oyunların sanal aygıtları kabul etmesi garanti edilmez. Kaldırma işlemi Windows **Ayarlar → Uygulamalar → FakerInput → Kaldır** üzerinden yapılır.

## Güncelleme

1. **Güncellemeleri kontrol et** düğmesine basın.
2. Yeni sürüm varsa güncellemeyi onaylayın.
3. LANDesk paketi indirip doğrular ve yeni sürümle yeniden açılır.

Güncelleme sırasında uzak bağlantılar kapanır; ardından hedefe yeniden bağlanabilirsiniz. LANDesk ayarları ve kayıtlı cihazları korur. Güncellemeyi her bilgisayarda ayrı başlatın.

## Sorun giderme

| Durum | Kontrol |
| --- | --- |
| Bilgisayar listede görünmüyor | Hedefte paylaşımı açın, cihazların aynı yerel ağda olduğunu kontrol edin ve aramayı yenileyin. Gerekirse IP ile ekleyin. |
| Bağlantı kurulamıyor | Hedefte LANDesk'in açık kaldığını ve güvenlik duvarındaki Özel ağ iznini kontrol edin. Misafir Wi-Fi ağı cihazlar arasındaki erişimi engelleyebilir. |
| Görüntü var, giriş çalışmıyor | Ekran görüntüsüne tıklayın ve fare/klavye kontrolünü açın. Kendi bilgisayarınıza bağlandığınız yerel testte girişler kapalıdır. |
| Güncelleme tamamlanmıyor | İnternet bağlantısını ve uygulama klasörüne yazma iznini kontrol edin. |

## Mevcut kapsam

LANDesk bir önizleme sürümüdür. Birincil monitörü ve açık Windows masaüstünü destekler.

Windows kilit ve oturum açma ekranları, UAC, yönetici olarak çalışan pencereler, çoklu monitör, dosya aktarımı ve pano eşitleme kapsam dışındadır. Farklı ev ağları arasında internet üzerinden bağlantı sunmaz.

Uygulama kendini Windows başlangıcına eklemez. Bilgisayarı yeniden açtığınızda LANDesk'i başlatıp paylaşımı açın.

Kendi bilgisayarınıza bağlanarak görüntü aktarımını deneyebilirsiniz. Yerel giriş döngüsünü önlemek için bu testte fare ve klavye kontrolü kapalı kalır. FakerInput için gerçek tuş, tıklama ve oyun uyumluluğu hedef bilgisayarda ayrıca doğrulanmalıdır.

