---
layout: default
title: "Bölüm 06: Ad Serving (Reklam Sunucuları)"
---

# Bölüm 06: Ad Serving (Reklam Sunucuları)

Bu bölümde dijital reklamcılığın en kritik bileşenlerinden biri olan **Ad Server** (Reklam Sunucusu) teknolojisini inceleyeceğiz.

Ad Server'lar, reklamların nasıl "servis edildiği" yani kullanıcıya teknik olarak nasıl iletildiğinin temelini oluşturur.

---

## 💡 Arka Plan

### 📅 Ad Server'ın Tarihi ve Önemi

Ad server'lar dijital reklamcılığın **en eski ve en kritik bileşenlerindendir**.

- **İlk kullanım:** 1990'ların sonları
- **Günümüz:** Hâlâ reklam ekosisteminin merkezinde yer alır
- **Önem:** Tüm dijital reklam süreçlerinin temel taşı

### 🎯 Ad Server'ın Rolleri

Ad Server'lar üç temel görevi yerine getirir:

1. **Karar Verme:** Reklamların hangi kullanıcıya, ne zaman, hangi yaratıcıyla gösterileceğini belirler
2. **Performans Toplama:** Impression, tıklama, dönüşüm gibi metrikleri toplar
3. **İki Taraflı Kullanım:** Hem reklamveren hem yayıncı tarafında farklı şekillerde kullanılır

### 🔗 Modern AdTech ile İlişkisi

DSP, SSP, Ad Exchange gibi yeni platformlar ortaya çıksa da:

- Ad server hâlâ **kampanya yönetimi ve ölçümleme** için temel platformdur
- Targeting, frequency capping, bütçe yönetimi gibi özellikler ad server mantığından türetilmiştir

---

## 🖥️ Ad Server Nedir?

### 🔹 Tanım:

Bir **ad server**, dijital reklamcılıkta kullanılan temel bir AdTech platformudur.

### 📍 Görevleri:

1. **🎯 Karar Verme:** Hangi reklamın gösterileceğine karar vermek (targeting, kurallar, frekans sınırlaması vb.)
2. **📡 Sunma:** Reklamı kullanıcıya sunmak (ad serving)
3. **📊 Ölçme:** Gösterim, tıklama gibi performans verilerini toplamak ve raporlamak

### 💡 Basit Benzetme:

**Ad servers** = (reklamlar/creatives) için **WordPress** = (içerik/articles) için

**Yani:**
- WordPress bir sitenin **içeriklerini** yönetir
- Ad server ise sitenin **reklamlarını** yönetir

---

## 👥 Kimler Ad Server Kullanır?

### 📰 Publishers (Yayıncılar)
**Siteler, uygulamalar** için:
- Kendi envanterlerini yönetmek
- Reklam göstermek

### 📢 Advertisers / Agencies (Reklamverenler / Ajanslar)
**Kampanya yönetimi** için:
- Kendi reklam kreatiflerini yönetmek
- Kampanyaları optimize etmek
- Farklı sitelerde reklam dağıtmak

### 🔄 İki Tür Ad Server:

- **📰 Publisher's Ad Server** (first-party ad server)
- **📢 Advertiser's Ad Server** (third-party ad server)

---

## ⚙️ Ad Server'lar Nasıl Çalışır?

### 🔄 Temel Süreç:

**Ad Ops ekibi** kampanyayı ad server'a yükler 
↓
**Ad server** yayıncı sitenin reklam slotunda hangi reklamın gösterileceğine karar verir 
↓
**Gösterimi** yapar 
↓
**Raporlar** oluşturur

### 📊 Özet:
**Karar verme + Sunma + Ölçme** süreçlerinin tamamı ad server ile gerçekleşir.

---

## 🔗 Reklamveren–Yayıncı İlişkisi

### 📅 1990'lar - 2000'ler Arası Dönem

Online reklamcılığın ilk dönemlerinde bir kampanyayı yürütmek **manuel bir süreçti** ve yalnızca reklamveren ile yayıncı arasındaki **doğrudan iletişimi** içeriyordu.

### 🤝 Temel İlişki:

**📢 Reklamveren:**
> "Bir ürün veya hizmeti tanıtmak ister, bu yüzden yayıncının web sitesinde reklam alanı satın alır."

**⬅️➡️**

**📰 Yayıncı:**
> "Web sitesini (veya uygulamasını) paraya çevirmek ister, bu yüzden reklam alanını reklamverenlere satar."

### 🖥️ Birinci Taraf Ad Server'ların Devreye Girişi

Ardından, yayıncının reklam sunucusu (ad server) reklamverenlerin kampanyalarını yürütmelerine ve raporlamalarına yardımcı olmak için kullanılmaya başlandı.

---

## 🚀 Kampanya Yürütme: Öncesi ve Sonrası

### 📋 Temel İşleyiş Adımları:

#### 1️⃣ **Insertion Order (IO) İmzalanması**
**Reklamveren → Yayıncı**

Bu belge (genellikle bir sözleşme) kampanyanın koşullarını belirtir:
- 📅 **Yayın tarihleri** (başlangıç – bitiş)
- 📍 **Placement** (reklamın nerede görüneceği)
- 📐 **Reklam formatı ve boyutu**
- 💰 **Fiyatlandırma modeli** (CPM, CPC gibi)
- 📝 **Diğer detaylar**

#### 2️⃣ **Kreatif Gönderimi**
Reklamveren **kreatif listesini** (genellikle Excel/Google Sheet dosyası) yayıncıya gönderir.

#### 3️⃣ **Kampanya Kurulumu**
Yayıncının **AdOps ekibi**, kampanyayı kendi reklam sunucusunda kurar.

#### 4️⃣ **Reklam Yayını**
Reklam yayına girer ve yayındaki sitede/ana sayfada görünür.

#### 5️⃣ **Raporlama**
Kampanya başladıktan sonra, yayıncı reklamverene **düzenli performans raporları** gönderir.

**Raporlarda yer alan metrikler:**
- 📊 **Gösterimler** (impressions)
- 🖱️ **Tıklamalar** (clicks)
- 📈 **Diğer performans verileri**

---

## 🔄 Ad Trafficking vs AdOps

### 🤔 Sık Karıştırılan Terimler

**Ad trafficking** ve **AdOps** terimleri sık sık birbirine karıştırılır, ancak aralarında önemli bir fark vardır.

### 📋 Ad Trafficking (Reklam Trafiği Yönetimi)

**Ad trafficking**, ad sunucuları ve/veya diğer AdTech platformları tarafından yürütülen kampanyaların:
- 🏗️ **Kurulması**
- 👁️ **İzlenmesi** 
- ⚡ **Optimize edilmesi**

sürecine verilen isimdir.

### 👥 AdOps (Advertising Operations)

**AdOps**, kampanyaları kurmak, izlemek ve optimize etmekten **sorumlu kişilerdir**.

### 📊 Özet Fark:

| **Terim** | **Ne İfade Eder** | **Odak** |
|-----------|-------------------|----------|
| **AdOps** | İnsanlar | Kampanya yönetiminden sorumlu ekip |
| **Ad Trafficking** | Süreç | Kampanya kurulum ve yönetim süreci |

> **💡 Kısaca:** AdOps **insanlara**, ad trafficking ise **sürece** atıfta bulunur.

---

## 📰 Birinci Taraf (Yayıncının) Ad Sunucusu

### 🔹 Temel Görevler:

Bir yayıncının ad sunucusu, **web sitesindeki reklam alanlarını doldurmakla** görevlidir.

**Reklam kaynaklarını eşleştirme:**
- 🎯 **Doğrudan kampanyalar**
- ⚡ **Gerçek zamanlı açık artırma (RTB)** süreçleri
- 💼 **Diğer medya satın alma** işlemleri

### ⚙️ Nasıl Çalışır:

1. **🎯 Karar Verme:** Kampanyanın hedefleme parametrelerine göre hangi reklamların gösterileceğine karar verir
2. **📡 Sunma:** Bu reklamları kullanıcıya sunar
3. **📊 Raporlama:** Performansları hakkında rapor oluşturur

### 📈 Envanter Tahmini Özelliği:

Ad sunucularının önemli bir özelliği **envanter tahminidir**:

- 🔮 **Gelecek Envanter:** Yayıncının gelecekte ne kadar envantere sahip olacağını tahmin eder
- 📊 **Performans Tahmini:** Reklam kampanyalarının mevcut ve geçmiş verilere göre performansını öngörür

### 🔄 Üçüncü Taraf Ad Server'lara Geçiş:

Kısa süre sonra, **reklamverenler** kendi kampanyalarının performansını ölçmek için ad sunucularını kullanmaya başladı. 

Bu ad sunucuları **üçüncü taraf ad sunucusu** veya **reklamverenin ad sunucusu** olarak bilinir.

---

## 📢 Üçüncü Taraf (Reklamverenin) Ad Server'ları

### 🚀 Yeni Süreç Akışı:

#### 1️⃣ **Insertion Order (IO) İmzalanması**
**Reklamveren → Yayıncı**

#### 2️⃣ **Ad Tag Oluşturma**
**Reklamverenin AdOps ekibi** kampanya için **ad tag'lerini** oluşturur ve **yayıncının AdOps ekibine** gönderir.

#### 3️⃣ **Kampanya Kurulumu**
**Yayıncının AdOps ekibi** kampanyayı yayıncının ad server'ında **reklamverenin ad tag'lerini** kullanarak kurar.

### 📚 Terim Açıklamaları:

| **İngilizce** | **Türkçe** | **Açıklama** |
|---------------|------------|--------------|
| **Advertiser's ad server** | Reklamverenin ad server'ı | Üçüncü taraf ad server |
| **Publisher's ad server** | Yayıncının ad server'ı | Birinci taraf ad server |
| **Third-party ad server** | Üçüncü taraf ad server | Reklamverenin kullandığı |
| **First-party ad server** | Birinci taraf ad server | Yayıncının kullandığı |

---

## 🔧 Üçüncü Taraf Ad Server'ların Doğuşu

### ⚠️ Reklamverenlerin Karşılaştığı Zorluklar:

Reklamverenlerin yayıncılarla doğrudan çalışırken karşılaştığı temel sorunlar:

#### 🚫 **Sınırlı Erişim**
- Tek bir kampanyanın sınırlı erişimi

#### 📊 **Raporlama Karmaşası**
- Kampanyayı farklı yayıncılar arasında tek bir yerden ölçmenin mümkün olmaması

#### ❓ **Raporlama Doğrulaması**
- Yayıncı tarafından sağlanan raporları doğrulamanın bir yolunun olmaması

### 📈 Online Reklamcılığın Patlama Dönemi

Ad server'ın icadı bu zorlukların çoğunu otomasyon yoluyla çözmüş olsa da, **reklamverenler için yeni zorluklar** ortaya çıktı.

**Sorunlar:**
- 🌊 **Yayıncı Patlaması:** Çok daha fazla yeni yayıncı pazara girmeye başladı
- ⚠️ **Güvenilirlik Sorunu:** Bunların hepsi güvenilir değildi
- 📉 **Güven Kaybı:** Yayıncılar ve ad network'ler tarafından oluşturulan raporlara artık güvenilemez hale geldi

---

## 🛡️ Bağımsız Reklam Sunucuları Çözümü

### 💡 Çözüm:

Reklamverenler, **birden fazla yayıncı ve reklam ağında** çalışan kampanyalarından **bağımsız raporlar** elde etmek için **bağımsız reklam sunucuları** kullanmaya başladılar.

> **📝 Not:** Bugün **üçüncü taraf reklam sunucusu** (reklamverenin reklam sunucusu) olarak bilinen sistemler.

### 🎯 Üçüncü Taraf Ad Server'ın Faydaları:

#### 📊 **Merkezi Performans Takibi**
Tüm kampanyanın performansını (gösterimler, tıklamalar, dönüşümler vb.) **tüm yayıncılar arasında tek bir sistemde** takip etmek.

#### 👥 **Erişim Ölçümü**
Yayıncılar arası **ortak izleyiciyi (co-viewership)** hesaba katarak kampanyanın erişimini ölçmek.

#### ✅ **Raporlama Doğrulaması**
Yayıncılar tarafından sağlanan raporları **doğrulamak**.

---

## 🔄 Üçüncü Taraf Ad Server İşleyiş Şeması

### 📋 Adım Adım Süreç:

#### 1️⃣ **Sözleşme İmzalama**
**Reklamveren ↔ Yayıncı**
- 📄 **Ek Yerleştirme Formu (IO)** imzalanır

#### 2️⃣ **Reklam Etiketleri Oluşturma**
**Reklamverenin (3. taraf) reklam sunucusu**
- 🏷️ **Ad Ops ekibi** kampanya için **reklam etiketlerini (tags)** oluşturur

#### 3️⃣ **Dosya Transferi ve Kurulum**
**Reklamverenin Ad Ops ekibi** şunları yayıncının Ad Ops ekibine gönderir:
- 🏷️ **Etiketler**
- 📊 **Gösterim piksel'leri**
- 🖱️ **Tıklama takipçileri**

**Yayıncının Ad Ops ekibi:**
- 🏗️ Kampanyayı yayıncının reklam sunucusunda kurar
- 📝 Bu işleme **ad trafficking** (reklam trafiği yönetimi) denir

#### 4️⃣ **Reklam Sunumu**
**Reklam alanı (ad slot)**
- 📡 Yayıncının sitesinden her reklam isteği gönderildiğinde
- 🖥️ Reklam alanı reklam sunucusundan reklamı yükler

---

## ⚡ Ad Server Nasıl Çalışır?

Artık bir reklam sunucusunun ne olduğunu ve neyle sorumlu olduğunu bildiğimize göre, **mekaniklerine** bir göz atalım.

---

### 📰 Yayıncının Ad Server'ı Nasıl Çalışır?

#### 🔄 Adım Adım Süreç:

**1️⃣ Kullanıcı Ziyareti**
- 👤 Bir kullanıcı bir web sitesini ziyaret eder
- 🌐 Tarayıcı, sayfanın içeriğini (HTML) istemek için **yayıncının web sunucusuna** bir istek gönderir

**2️⃣ İçerik Yükleme**
- 📄 Yayıncının web sunucusu **HTML'yi** geri gönderir
- 🖥️ Tarayıcı **sayfa içeriğini** oluşturmaya başlar

**3️⃣ Reklam İsteği**
- 📡 Sayfada bulunan **reklam alanını** doldurmak için yayıncının reklam sunucusuna bir **reklam isteği** gönderilir

**4️⃣ Kampanya Seçimi**
- 🎯 Yayıncının reklam sunucusu, **kullanıcı hakkında elde edilen bilgilere** dayanarak bir **reklam kampanyası** seçer

**5️⃣ Reklam Sunumu**
- 📜 Yayıncının reklam sunucusu **JavaScript etiketini** web sitesine geri gönderir
- 👁️ **Reklam kullanıcıya gösterilir**

---

### 📢 Reklamverenin Ad Server'ı Nasıl Çalışır?

#### 🔄 Genişletilmiş Süreç:

**1️⃣ Kullanıcı Ziyareti**
- 👤 Bir kullanıcı bir web sitesini ziyaret eder
- 🌐 Tarayıcı, sayfanın içeriğini (HTML vb.) istemek için **yayıncının web sunucusuna** bir istek gönderir

**2️⃣ İçerik Yükleme**
- 📄 Yayıncının web sunucusu **HTML'i** geri gönderir
- 🖥️ Sayfanın içeriği **yüklenmeye başlar**

**3️⃣ Reklam İsteği**
- 📡 Sayfadaki **reklam alanını** doldurmak için yayıncının reklam sunucusuna bir **reklam isteği** gönderilir

**4️⃣ Kampanya Seçimi**
- 🎯 Yayıncının reklam sunucusu, **kullanıcı hakkında elde edilen bilgilere** dayanarak gösterilecek **reklam kampanyasını** seçer

**5️⃣ Markup Gönderimi**
- 📜 Yayıncının reklam sunucusu, reklam alanına yerleştirilen **reklam markup'ını** (yani kodu) geri gönderir
- 🔗 Bu kod, **reklamverenin reklam sunucusuna işaret eden bir URL** içerir

**6️⃣ Üçüncü Taraf İsteği**
- ⚡ Reklam markup'ı, **reklamverenin reklam sunucusuna** bir istek gönderir (yani kod çalışır)
- 📊 Bir **gösterim (impression)** sayılır

**7️⃣ Final Reklam Sunumu**
- 📜 Reklamverenin reklam sunucusu, **markup'ı** yayıncının sitesine geri gönderir
- 👁️ **Reklam kullanıcıya gösterilir**

---

## 🔄 Birinci Taraf vs Üçüncü Taraf Ad Sunucuları

### 💡 Temel Benzerlik:

Birinci taraf ve üçüncü taraf ad sunucuları **temelde aynı tür teknolojidir**; ancak yayıncılar ve reklamverenler için **farklı sorumluluklar** üstlenirler.

---

### 📊 Detaylı Karşılaştırma:

| **Özellik** | **📰 Birinci Taraf Ad Sunucusu<br>(Yayıncının Ad Sunucusu)** | **📢 Üçüncü Taraf Ad Sunucusu<br>(Reklamverenin Ad Sunucusu)** |
|-------------|-----------------------------------------------------------|----------------------------------------------------------|
| **🎯 Temel Görev** | AdOps ekiplerinin web sitesindeki reklam alanlarını yönetmesi, birden fazla doğrudan kampanya yürütmesi ve SSP gibi diğer platformlardan gelen üçüncü taraf etiketlerini yönetmesi | Kampanyanın dahil olduğu tüm sitelerde performansı takip etmesi (erişim, gösterimler, tıklamalar, dönüşümler), ROI hesaplaması ve dönüşümleri doğru yayıncılara atması |
| **📈 Analitik & Raporlama** | Yayıncıların envanter doluluk oranlarını tahmin etmesi, gelir ve faturalama raporları sunması ve farklı kaynaklardan gelen talebin verimliliğini analiz etmesi | Reklamverenin gelecekteki medya satın alımlarını optimize etmesi, hangi sitelerin ve hedeflemelerin işe yaradığını belirlemesi ve A/B testleri yapması |
| **🔮 Tahmin & Optimizasyon** | Yayıncıların belirli hedefleme kriterlerini karşılayan trafik & envanter miktarını öngörmesi | Reklamverenlerin performans metriklerini denetlemesi ve doğrulaması |

⸻

## 🔄 Yayıncı Ad Sunucusu ile Ad Serving Süreci

İlk örnek, ad sunumunun yalnızca bir yayıncı ad sunucusu kullanıldığında nasıl çalıştığını göstermektedir:

### 📋 İşleyiş Adımları

**🍪 Çerez Kullanımı:** Birinci taraf çerezi kullanılır.

1. **📱 Kullanıcı İsteği:** Kullanıcı bir web sitesini ziyaret ettiğinde tarayıcı, yayıncının web sunucusuna HTML içeriğini almak için bir istek gönderir.
Web sunucusu HTML’yi döndürür ve sayfa yüklenmeye başlar.

Sayfada bulunan reklam alanının kodu, tarayıcının yayıncının ad sunucusuna bir reklam isteği göndermesini tetikler.
Yayıncının ad sunucusu, kullanıcı hakkında elde ettiği bilgilere dayanarak uygun bir kampanya seçer.
Ad sunucusu, reklamverenin reklam etiketi (markup) ve kreatifini geri gönderir.
Tarayıcı bu kreatifi yükleyip reklam alanında görüntüler.
Gösterim bu süreçte sayılmış olur.

---

## 🔄 Yayıncı + Reklamveren Ad Sunucusu ile Ad Serving Süreci

İkinci örnek, hem yayıncı hem de reklamveren ad sunucusunun sürece dahil olduğu ad sunma yapısını göstermektedir:

### 📋 İşleyiş Adımları

**🍪 Çerez Kullanımı:** Hem birinci taraf hem üçüncü taraf çerezleri kullanılabilir.

1. **📱 Kullanıcı İsteği:** Kullanıcı web sitesine gider ve tarayıcı yayıncının web sunucusundan HTML kodunu ister.
Web sunucusu HTML’yi döndürür ve sayfa yüklenmeye başlar.

Reklam alanının kodu, yayıncının ad sunucusuna bir reklam isteği gönderir.
Yayıncının ad sunucusu kampanya eşleştirmesi yapar, gösterimi sayar ve reklam markup’ını döndürür.

Bu reklam markup’ı, tarayıcının bu kez reklamverenin (üçüncü taraf) ad sunucusuna bir istek göndermesini tetikler. Buna “piggybacking” denir.

Reklamveren ad sunucusu:
	•	kampanyayı seçer,
	•	gösterimi sayar,
	•	kreatifin bulunduğu CDN’e bir bağlantı içeren markup’ı döndürür.

Tarayıcı CDN’e gidip kreatifi çeker ve reklamı kullanıcıya gösterir.

⸻

Bir Ad Sunucusunun Anatomisi

Aşağıda, yukarıdaki diyagramlarda geçen ad sunma bileşenlerinin açıklamaları yer almaktadır.

Reklam Etiketleri (Ad Tags)

Bir reklam etiketi, bir reklamın bir reklam alanına yerleştirilmesini sağlayan kod parçasıdır.
Ad etiketleri, uygulama yöntemine göre farklı türlerde olabilir.

Aşağıda en yaygın reklam etiketi türleri, kullanım amaçları ve sundukları avantaj–dezavantajlar açıklanmaktadır (örneğin: JavaScript ad tags).

⸻

JavaScript Reklam Etiketleri (JavaScript Ad Tags)

Kullanım:
JavaScript reklam etiketleri, masaüstü veya mobil tarayıcıda web sayfalarında display reklamların sunulması için kullanılır.
Mobil uygulamalarda da kullanılabilirler; bu durumda genellikle özel etiketler veya MRAID (Mobile Rich Media Ad Interface Definition) kullanılır.

Uygulama:
JavaScript reklam etiketleri doğrudan yayıncının sayfa koduna yerleştirilir.

Avantajlar:
	•	Reklamlar yayıncının web sitesiyle etkileşime girebilir.
	•	Görüntülenebilirlik (viewability) takip edilebilir.
	•	Reklamlar, içeriğin yüklenmesi sırasında veya sonrasında yüklenebilir (uygulamaya bağlıdır).

Dezavantajlar:
	•	Reklamlar, yayıncının web sitesi içeriğini değiştirebilir ve sitenin bozulmasına neden olabilir.
	•	Reklamlar güvenlik riskleri oluşturabilir; örneğin JavaScript enjeksiyonu yoluyla kötü amaçlı yazılım yüklenebilir ve kullanıcıların form verileri, şifreleri, e-posta adresleri gibi hassas bilgiler ele geçirilebilir.
Örneğin: Magecart saldırısı, 380.000 müşterinin kredi kartı bilgilerinin çalınmasına yol açmıştır.

Bir JavaScript reklam etiketi örneği:

<script type="text/javascript"><!--
google_ad_client = "pub-1111111111";
/* 160x600 - TOP */
google_ad_slot = "12345";
google_ad_width = 160;
google_ad_height = 600;
//-->
</script>
<script type="text/javascript"
src="http://pagead2.googlesyndication.com/pagead/show_ads.js">
</script>


⸻

Iframe Reklam Etiketleri (Iframe Ad Tags)

Kullanım:
Masaüstü veya mobil tarayıcıda web sayfalarında display reklam sunumu için kullanılır.

Uygulama:
Iframe reklam etiketleri, yayıncının sayfa koduna eklenen HTML iframe etiketleridir.
Iframe, içindeki reklam kodunu tamamen izole eder ve bu sayede reklamın sayfanın geri kalanıyla etkileşime girmesini engeller.

Avantajlar:
	•	Yayıncıyı, reklam kodlarının web sitesinin içeriğini değiştirmesinden korur.
	•	JavaScript kodunu iframe içinde izole ederek güvenliği artırır.
	•	Reklamlar içeriğin geri kalanından sonra yüklenebilir; bu da sayfa yükleme süresini iyileştirebilir.

Dezavantajlar:
	•	Yayıncı sitesindeki içerikle sınırlı etkileşim — genişletilebilir reklamlar için ek JavaScript gerekir.
	•	Viewability (görüntülenebilirlik) takip edilmesi zordur.

Bir iframe reklam etiketi örneği (OpenX):

<iframe id="a62ae7d3" name="a62ae7d3"
src="http://delivery_server_domain/w/1.0/afr?auid=6635&cb=INSERT_RANDOM_NUMBER_HERE&rnd=5&r=3"
frameborder="0" scrolling="no" width="728" height="90">
<a href="http://delivery_server_domain/w/1.0/ct?cs=aed22faf&cb=INSERT_RANDOM_NUMBER_HERE"
target="_blank">
<img
src="http://delivery_server_domain/w/1.0/ai?auid=6635&cs=aed22faf&cb=INSERT_RANDOM_NUMBER_HERE"
border="0" alt="" /></a></iframe>


⸻

SafeFrame

JavaScript ve iframe reklam etiketlerinde görülen sorunları çözmek için IAB tarafından yeni bir standart tanıtılmıştır: SafeFrame.

SafeFrame nedir?
SafeFrame, iframe ve JavaScript reklam etiketlerinin avantajlarını birleştirip birçok dezavantajlarını ortadan kaldıran bir IAB standardıdır.

SafeFrame reklam alanları, reklamı iframe içinde yükler; ancak bir API aracılığıyla bu iframe’in reklamveren ile kontrollü şekilde etkileşime girmesine izin verir.

Bu sayede:
	•	Reklamveren, reklam alanını genişletebilir veya viewability ölçümleri yapabilir.
	•	Yayıncı ise site bütünlüğünü korur; reklam kodu site içeriğini değiştiremez.
	•	Kullanıcıların hassas bilgileri korunur.

⸻

SafeFrame Nasıl Çalışır?

SafeFrame uygulaması aşağıdaki şekilde çalışır:
	1.	Kullanıcı yayıncının web sitesine erişir ve tarayıcı, içeriği ve SafeFrame işaretlemelerini almak için yayıncının web sunucusuna bir istek gönderir.
	2.	SafeFrame (JavaScript), SafeFrame API’si ile birlikte bir iframe yükler ve bu iframe’in yayıncı sitesiyle kontrollü şekilde etkileşime geçmesine izin verir.
	3.	Reklam işlenir ve kullanıcıya gösterilir.
	4.	Aynı zamanda, görüntülenebilirlik (viewability) ve ölçüm satıcıları tarafından veri toplanır ve reklamverenlere raporlanır.

SafeFrame ile yüklenen reklamların iframe içinde tamamen izole edildiğini unutmamak önemlidir — yani üçüncü taraf ve reklamverenin ad sunucuları iframe içinde JavaScript çalıştırabilir, ancak yayıncının web sitesini etkileyemez. Yayıncı sitesiyle etkileşim sadece SafeFrame API tarafından izin verilen yöntemlerle yapılabilir; örneğin görüntülenebilirlik ölçümü gibi belirli işlemler mümkündür.

⸻

VAST ve VPAID (Video Reklamları İçin)

Video reklam sunumunda, IAB tarafından tanımlanan iki format kullanılır:
VAST (Video Ad-Serving Template) ve VPAID (Video Player Ad-Serving Interface Definition).

VAST nedir?
VAST, video reklamlarının (örneğin YouTube benzeri video oynatıcı içi reklamlardan) video ad sunucularından alınarak birçok farklı cihazda (masaüstü, mobil, tablet vb.) oynatılmasını sağlayan bir XML şemasıdır.

VPAID nedir?
VPAID, video reklam birimleriyle video oynatıcıların karşılıklı etkileşim kurmasını sağlayan bir JavaScript parçasıdır.

⸻

IMG Reklam Etiketleri (IMG Ad Tags)

IMG reklam etiketleri HTML etiketleridir ve iframe etiketlerine benzer.

Kullanım:
Bu etiketler genellikle mobil uygulamalarda display reklam göstermek için veya tarayıcının JavaScript çalıştırmadığı durumlarda yedek (fallback) olarak kullanılır.

Uygulama:
Çoğu AdTech platformu ve yayıncı, tam HTML belgeleri yerine yalnızca HTML/IMG kod snippet’lerini kabul eder (örneğin <html>, <head> veya <title> etiketleri olmadan).

HTML/IMG reklam etiketi örneği:

<a href="https://www.clearcode.cc/">
  <img src="http://clearcode250x250.jpg">
</a>


⸻

Avantajlar
	•	HTML/IMG etiketleri basit bir yapıya sahiptir ve teknik sorunlarla karşılaşmadan kolayca tarayıcı ve uygulamalarda görüntülenebilir.
	•	İçerik dağıtım ağı (CDN) kullanarak görseller daha hızlı yüklenebilir; bu da reklamın görüntülenme olasılığını artırır.

⸻

Dezavantajlar
	•	HTML/IMG reklam etiketleri zengin medya reklamlarını (ör. genişleyebilir veya etkileşimli reklamlar) destekleyemez.

⸻

Reklam Etiketlerini Takip Etmek İçin Kullanılan Spreadsheet’ler

Reklamverenler, kampanyalarında kullanılan reklam etiketlerini takip etmek için genellikle spreadsheet’ler oluşturur.

Tipik bir spreadsheet şu bilgileri içerir:
	•	Yerleştirme listesi
	•	Her yerleştirme için ilgili reklam etiketi

Bu işlem manuel ve hata yapmaya açık olsa da, programatik olmayan display kampanyalarında (yayıncı ile reklamveren arasındaki doğrudan anlaşmalar) ve bazı self-serve AdTech platformlarında hâlâ yaygın kullanılan yöntemdir.

⸻

Ad Markup (Reklam İşaretlemesi)

Ad markup, bir ad sunucudan veya başka bir AdTech platformundan (ör. SSP, DSP vb.) bir reklam etiketi aracılığıyla alınan ve bir reklam alanında (ad slot) işlenen bir kod parçasıdır.

Aşağıdaki görselde temel akış gösterilir:
	1.	Reklam alanının (ad slot) kodu, tarayıcının bir AdTech platformuna (ad server, SSP vb.) istek göndermesini tetikler.
	2.	AdTech platformu reklam işaretlemesini (ad markup) geri döndürür.
	3.	Reklam işaretlemesi, kreatif dosyasını ve izleme piksellerini yüklemek için gereken çağrıları yapar.

⸻

Ad Markup’ın İki Ana Sorumluluğu
	1.	Reklam kreatif dosyasını (ör. banner görseli, video) reklam alanına yüklemek.
	2.	İzleme piksellerini yükleyerek gösterimi (impression) takip etmek. Bu takip şu amaçlarla yapılır:
	•	Ölçümleme (measurement)
	•	Reklam doğrulama (ad verification)
	•	Görüntülenebilirlik ölçümü (viewability)
	•	Diğer analitik işlemler

⸻

Basit Bir Ad Markup Örneği

<a href="http://landingpage.com/">
  <img src="http://host-with-creatives.com/ads/banner.jpg" />
</a>


⸻

Bölüm Özeti (Chapter Summary)
	•	Ad serving, çevrimiçi reklamcılığın temel süreçlerinden biridir.
	•	Birinci taraf (publisher) ad server, yayıncılar tarafından web sitelerindeki reklam alanlarını yönetmek, doğrudan kampanyalardan gelen reklamları sunmak, RTB gibi diğer kampanyaları yönetmek ve performans raporlamak için kullanılır (örn. gösterimler ve tıklamalar).
	•	Üçüncü taraf (advertiser) ad server, reklamverenler tarafından kreatiflerini yönetmek, yayıncılara göndermek ve kampanyalarının performansı hakkında veri toplamak için kullanılır.

⸻



### 📋 Özet Farklar:

#### 📰 **Birinci Taraf (Yayıncı) Odaklı:**
- 🏗️ **Envanter yönetimi**
- 💰 **Gelir optimizasyonu**
- 📊 **Doluluk oranları**

#### 📢 **Üçüncü Taraf (Reklamveren) Odaklı:**
- 📈 **Performans takibi**
- ✅ **Doğrulama ve denetim**
- 🎯 **Kampanya optimizasyonu**

---

## 🔧 Teknik Alan & Ad Server Anatomisi

Ad serving sürecinin **teknik detayları** ve **sistem mimarisi** hakkında daha ayrıntılı bilgi için, gelişmiş konular bölümüne bakabilirsiniz.

Bu bölümde ele alınan temel konular:
- 🖥️ **Server mimarisi**
- 📡 **API entegrasyonları**
- 🔄 **Veri akış süreçleri**
- ⚡ **Performans optimizasyonu**

---

## 🎓 Bölüm Özeti

Bu bölümde Ad Serving (Reklam Sunucuları) teknolojisinin temellerini öğrendik:

### **📚 Öğrendiklerimiz:**

1. **🖥️ Ad Server Tanımı** - Dijital reklamcılığın temel platformu
2. **🔄 İki Tür Ad Server** - Birinci taraf (yayıncı) vs Üçüncü taraf (reklamveren)
3. **🚀 Kampanya Süreçleri** - IO imzalamadan reklam yayınına kadar
4. **⚙️ Teknik Çalışma** - Adım adım reklam sunumu süreci
5. **📊 Karşılaştırma** - Her iki ad server türünün avantajları

### **🔑 Ana Çıkarımlar:**

- **Temel Rol:** Ad server'lar dijital reklamcılığın omurgasını oluşturur
- **İki Perspektif:** Yayıncı ve reklamveren farklı ihtiyaçlar için kullanır
- **Otomasyon:** Manuel süreçleri otomatikleştirerek verimliliği artırır
- **Güvenilirlik:** Bağımsız ölçüm ve doğrulama imkanı sağlar

### **📈 Sonraki Bölümlerde:**

- Hedefleme ve bütçe kontrolü mekanizmaları
- İzlenim, tıklama ve dönüşüm takibi
- Programatik satın alma süreçleri
- Gerçek zamanlı teklif verme (RTB) sistemleri

---

[⬅️ Bölüm 05: Başlıca Dijital Reklam Mecraları ve Kanalları](/The-AdTech-Book/bolumler/05-baslica-dijital-reklam-mecralari-ve-kanallari) | [🏠 Ana Sayfa](/The-AdTech-Book/) | [➡️ Bölüm 07: Hedefleme ve Bütçe Kontrolü](/The-AdTech-Book/bolumler/07-hedefleme-ve-butce-kontrol)