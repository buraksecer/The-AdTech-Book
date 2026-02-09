---
layout: default
title: "Bölüm 07: Hedefleme ve Bütçe Kontrolü"
---

# Bölüm 07: Hedefleme ve Bütçe Kontrolü

Bu bölümde dijital reklamcılıkta **hedefleme (targeting)** ve **bütçe kontrolü** mekanizmalarını inceleyeceğiz.

Hedefleme, reklamverenlerin doğru kullanıcılara, doğru zamanda ve doğru içerikle reklam göstermesini sağlayan kritik bir teknolojidir.

---

## 💡 Arka Plan

### 📅 Hedeflemenin Tarihi ve Önemi

Çevrimiçi reklamcılık bağlamında **hedefleme (targeting)**, belirli bir dizi kritere uyan kullanıcılara reklamların gösterilmesini ifade eder.

**Örnek Senaryo:**
Bahçe ürünleri satan bir reklamverenin hedef kitlesinin ABD'nin kırsal bölgelerinde yaşayan, 30–50 yaş aralığındaki kişiler olduğunu varsayalım. Bu durumda reklamveren, reklamlarını bu kriterlere uyan kişilere göstermek ister.

### 🔄 Hedeflemenin Evrimi

**Geleneksel Yaklaşım:**
Reklamveren ile yayıncı arasındaki **doğrudan anlaşmalarda (direct deals)** hedefleme, geleneksel olarak reklam sunucuları (ad servers) üzerinden yapılırdı.

**Süreç:**
1. Reklamveren, hedefleme kriterlerini **Insertion Order (IO)** içinde tanımlar
2. Örneğin: Yayıncının sitesinde reklamların hangi sayfalarda veya hangi bölümlerde gösterileceğini belirtir
3. Yayıncının **AdOps ekibi**, bu hedefleme kriterlerini yayıncının reklam sunucusunda (birinci taraf / first-party ad server) yapılandırır

**Modern Yaklaşım:**
Hedefleme hâlâ reklam sunucuları aracılığıyla yapılmakla birlikte, günümüzde birçok başka AdTech platformu (ör. **DSP'ler** ve **SSP'ler**) de hedefleme yetenekleri sunmaktadır.

### 🎯 Bu Bölümün Kapsamı

Bu bölümde, hedeflemeyi **reklam sunucuları (ad servers)** bağlamında ele alacağız.

Bir kampanya için hedefleme kriterleri belirleyerek, reklamveren kendisi için hangi web trafiğinin **relevant (uygun/değerli)** olduğunu seçebilir.

---

## 🎯 Hedefleme Nedir?

### 🔹 Tanım:

**Hedefleme (Targeting)**, dijital reklamcılıkta belirli kriterlere uyan kullanıcılara reklamların gösterilmesi sürecidir.

### 📍 Temel Amaç:

Reklamverenlerin:
- ✅ Doğru kullanıcılara ulaşması
- ✅ Reklam bütçelerini verimli kullanması
- ✅ Dönüşüm oranlarını artırması
- ✅ ROI (Return on Investment) değerini optimize etmesi

---

## 🌐 Bağlamsal Hedefleme (Contextual Targeting)

### 🔹 Tanım:

**Bağlamsal hedefleme**, reklamverenlerin ziyaretçi hakkında toplanan veriler yerine, **web sitesinin içeriğine dayalı** olarak ilgili reklamları göstermesine olanak tanır.

### 📚 Tarihsel Bağlam:

Bu hedefleme yöntemi, **dergi ve gazetelerde** yaygın olarak kullanılmaktadır. Örneğin, bir otomobil dergisinde otomobil reklamları görmek gibi.

### 💡 Temel Özellik:

Bağlamsal reklamlar, **kişisel verilere aşırı ihtiyaç duymadan** reklamı doğru şekilde hedeflemenin bir yoludur.

### 🎯 Kullanım:

Birçok reklamveren ve yayıncı, bağlamsal hedeflemeyi:
- ✅ **Tek başına** kullanır
- ✅ **Diğer hedefleme yöntemleriyle birlikte** kullanır

Çünkü bu yöntem belirli içerik türleri için oldukça etkilidir.

---

## ⚙️ Bağlamsal Hedefleme Nasıl Çalışır?

### 📋 Adım Adım Süreç:

#### 1️⃣ **Web Tarama (Web Crawling)**
- 🕷️ Bir **web crawler (tarayıcı)** URL'leri tarar
- 📊 İçerikleri ve reklam alanlarını **kategorize eder**

#### 2️⃣ **Kullanıcı Ziyareti**
- 👤 Bir ziyaretçi web sitesine erişir
- 📡 URL ile ilişkili bilgiler, **reklam isteği (ad request)** aracılığıyla yayıncının reklam sunucusuna (publisher's ad server) iletilir

#### 3️⃣ **Veri Aktarımı**
- 🔄 Bu reklam isteği ve bağlamsal bilgiler, **reklam borsaları (ad exchange)** ve **arz tarafı platformları (SSP)** gibi diğer AdTech platformlarına aktarılır

#### 4️⃣ **Teklif Verme**
- 💰 Reklam borsaları ve SSP'ler bu bilgileri, gösterim için teklif veren **talep tarafı platformlarına (DSP)** iletir

#### 5️⃣ **Reklam Gösterimi**
- 🎯 Kazanan DSP, reklamı yayıncıya geri gönderir
- 👁️ Reklam ziyaretçiye gösterilir

### 📊 Bağlamsal Hedeflemede Kullanılan Bilgiler:

Bağlamsal hedeflemede, sürecin her bir bileşeni, hangi reklamların gösterileceğini belirlemek için **web sitesi ve sayfa hakkındaki bilgileri** kullanır.

**Bu bilgiler şunları içerebilir:**
- 🌐 **URL**
- 🔑 **Anahtar kelimeler**
- 📄 **İçerik**
- 📂 **Kategoriler**
- 🏷️ **Etiketler (tags)**

### ✅ Bağlamsal Hedeflemenin Avantajları:

Bu yapı sayesinde:
- 🔒 **Kişisel kullanıcı verilerine ihtiyaç duyulmaz**
- 🎨 **Reklamlar, sayfanın içeriğiyle doğal olarak uyumlu olur**
- ⚖️ **Gizlilik ve regülasyonlara uyum kolaylaşır**

---

## 💎 Bağlamsal Hedeflemenin Faydaları

Bağlamsal hedefleme, diğer hedefleme yöntemlerine kıyasla oldukça basit gibi görünse de, reklamverenler ve yayıncılar için birçok önemli avantaj sunar:

### 🔒 **Gizlilik Uyumluluğu**
- Çoğu bağlamsal reklam **kişisel verilere dayanmaz**
- Bu da reklamverenlerin ve yayıncıların **GDPR** gibi gizlilik ve veri koruma regülasyonlarına maruziyetini azaltır

### 🛡️ **Marka Koruması (Brand Safety)**
- Bağlamsal reklamlar **daha güvenli marka koruması** sağlar
- Reklamlar, uygun içerik bağlamında gösterilir

### 📈 **Yüksek Performans**
- Yapılan çalışmalar, bağlamsal reklamların **satın alma niyetini %63 oranında artırabildiğini** göstermektedir

### 😊 **Kullanıcı Deneyimi**
- Davranışsal hedeflemeye dayalı reklamlara kıyasla **daha az rahatsız edici** bulunurlar
- Yine de kullanıcıların ilgi alanlarına dayanırlar

**Örnek:**
Akıllı telefonlarla ilgili makaleler okuyan kullanıcılara akıllı telefon tarifeleriyle ilgili reklamlar gösterilebilir.

---

## 🔑 Anahtar Kelimeler (Keywords)

### 🔹 Tanım:

**Anahtar kelimeler**, reklamverenler için değerli hedefleme değişkenleridir, çünkü web sitesi ziyaretçisinin **tükettiği içerik türü hakkında doğru bir resim** sunarlar.

### 🔍 Anahtar Kelime Tespiti:

Bir reklam sunucusu, belirli bir web sayfasında hangi anahtar kelimelerin bulunduğunu birkaç farklı yöntemle tespit edebilir:

#### 1️⃣ **Editör Etiketleri**
- 📝 Editör tarafından sayfada kullanılan ve içeriğin ana konularını vurgulayan **etiketler (tags)** aracılığıyla

#### 2️⃣ **Otomatik Çıkarma**
- 🤖 Sayfadaki anahtar kelimelerin **JavaScript** veya **sunucu taraflı web taraması (server-side crawling)** ile çıkarılması yoluyla

### ⚙️ Kullanım Süreci:

1. Bu anahtar kelimeler genellikle **ad tag'e** iletilir
2. Reklam sunucusu, **reklam isteği (ad request)** sırasında bu bilgileri alır
3. Hangi reklamın gösterileceğine karar verme sürecinde kullanır

### 💡 Örnek Senaryo:

**Senaryo:**
Bir reklamveren yeni bir akıllı telefon tarifesini tanıtmak istiyor.

**Hedefleme:**
- `smartphone`
- `mobile phone`

gibi anahtar kelimeleri içeren makaleleri okuyan ziyaretçileri hedefleyebilir.

---

## 📍 Reklam Alanı (Ad Slot) ve Reklam Pozisyonu (Ad Position)

### 🔹 Tanım:

Reklamverenler, **belirli boyutlara sahip** veya **web sayfasının belirli bir bölümünde yer alan** reklam alanlarında reklam göstermek isteyebilirler.

### 📐 Örnek Kriterler:

**Boyut:**
- 728×90 piksel boyutunda reklam alanları

**Konum:**
- Sayfanın üst kısmında (top of the page) konumlanan reklam alanları

### ⚠️ Önemli Not:

Bu tür hedefleme **oldukça geniş kapsamlı** olduğu için genellikle **diğer hedefleme yöntemleriyle birlikte** kullanılır.

---

## 🌐 Yayıncının URL'si (Publisher's URL)

### 🔹 Tanım:

Yayıncının URL'sine göre kullanıcıları hedeflemek, reklamverenlerin **basılı medyada (print media)** tüketicileri hedefleme biçimine oldukça benzer.

### 💡 Temel Mantık:

Belirli web sitelerinde reklam göstererek, reklamverenler:
- ❌ Yaş ve cinsiyet gibi demografik bilgiler yerine
- ✅ Kullanıcıların **ilgi alanlarına dayalı** olarak
- 🎯 çok daha geniş bir çevrim içi tüketici kitlesine ulaşabilirler

### 📊 Hedefleme Seviyeleri:

Reklamverenlerin web sitesi ziyaretçilerini hedefleyebileceği **iki seviye** vardır:

---

### 🌍 Domain (Alan Adı) Hedefleme

#### 🔹 Tanım:

Reklamverenler, hedef kitlelerini yayıncının **alan adı (domain)** üzerinden hedefleyebilir.

#### ⚠️ Kısıtlama:

Bu yöntem yalnızca, yayıncının **birden fazla farklı web sitesine sahip olduğu** doğrudan reklamveren–yayıncı ilişkilerinde geçerlidir.

#### 🔗 İlişkili Terim:

Bu yaklaşım genellikle reklam ağlarında kullanılan **run-on-site (ROS)** hedefleme ile ilişkilidir.

**ROS Modeli:**
Bu modelde reklamverenler, reklamlarını **belirli alan adlarında (domain'lerde)** gösterir.

---

### 📂 Bölüm (Section) ve URL'ler

#### 🔹 Tanım:

Reklamveren, sitenin **belirli bölümlerini (section)** hedeflemeyi tercih edebilir.

#### 💡 Örnek Senaryo:

**Durum:**
Bir site çok sayıda konuyu kapsıyorsa (örneğin bir haber sitesi)

**Hedefleme:**
Reklamveren yalnızca:
- 💻 **Teknoloji** bölümünü
- 🎬 **Eğlence** bölümünü

hedeflemek isteyebilir.

#### ⚠️ Teknik Zorluk:

**Sorun:**
Bu bölümler genellikle yalnızca URL üzerinden **net bir şekilde ayırt edilemez**.

**Çözüm:**
Bu nedenle yayıncının, reklam sunucusunun bu değişkeni hedeflemede kullanabilmesi için **bölüm adını (section name)** ad tag içinde göndermesi gerekebilir.

#### 🔗 İlişkili Terim:

Bu hedefleme yöntemi çoğu zaman reklam ağlarında kullanılan **run-on-network (RON)** hedefleme ile ilişkilidir.

**RON Modeli:**
RON hedeflemede reklamverenler, reklamlarını **belirli bir web sitesi grubunda** gösterir.

---

## 🌍 IP ve Coğrafi Konum (IP and Geolocation)

### 🔹 Tanım:

**Coğrafi konum hedeflemesi (geolocation targeting)**, kullanıcılara **mevcut konumlarına göre** reklam gösterilmesini ifade eder.

### 💡 Örnek Senaryo:

**Durum:**
Bir kullanıcı **Chicago'da** dizüstü bilgisayarından haber makaleleri okuyorsa

**Sonuç:**
Chicago bölgesindeki:
- 🏪 Mağazaları
- 🍽️ Restoranları
- 🛠️ Hizmetleri

tanıtan reklamları görmesi oldukça olasıdır.

---

## 🔍 Coğrafi Konum Nasıl Belirlenir?

### ❓ Soru:

Peki reklamverenler kullanıcıların nerede olduğunu nasıl bilir?

### ⚙️ Teknik Süreç:

#### 1️⃣ **Reklam İsteği**
- 📡 Reklam sunucusu, kullanıcının tarayıcısından gelen **reklam isteğini (ad request)** alır
- 🌐 Bu istek, kullanıcının **IP adresini** içerir

#### 2️⃣ **IP Eşleştirme**
- 🔍 IP adresi, **MaxMind** veya **Neustar** gibi harici veritabanları kullanılarak:
  - 🌍 **ülke**
  - 🗺️ **bölge**
  - 🏙️ **şehir**
  
  bilgileriyle eşleştirilir

#### 3️⃣ **Hedefleme**
- 🎯 Reklam sunucusu, kullanıcının konumunu belirleyerek **coğrafi hedefleme** yapabilir

---


## 📱 GPS ve Mobil Uygulamalarda Coğrafi Hedefleme

### 🔹 Gelişmiş Konum Tespiti:

**Yerel (Native) Mobil Uygulamalar:**
Yerel mobil uygulamalar, bir akıllı telefonun **GPS'inden alınan kesin enlem ve boylam bilgilerini** doğrudan reklam sunucusuna iletebilir.
### 🎯 Radius-Based Targeting (Yarıçap Bazlı Hedefleme):

Bu gibi durumlarda reklam sunucusu, kullanıcıları **belirli bir noktanın belirli bir yarıçapı içinde** hedefleyebilir.

**Örnek:**
Bir mağazanın **5 mil çevresindeki kullanıcılar** hedeflenebilir.

### ✅ GPS Hedeflemenin Avantajları:

Bu yaklaşım, **IP adresine dayalı konum tespitine kıyasla çok daha hassas ve doğru** bir coğrafi hedefleme sağlar.

### ⚠️ GPS Verilerinin Sınırlamaları:

Ancak şunu da belirtmek gerekir ki:
- ⚠️ GPS verileri dahi **zaman zaman hatalı olabilir**
- 🚨 Hatta bazı durumlarda **sahte (fraudulent) konum bilgileri** söz konusu olabilir

### 🔧 Doğruluk İyileştirme:

Konum verilerinin doğruluğunu artırmak için bazı veri şirketleri:
- 📊 **Farklı veri noktalarını**
- 🔍 **Sensörleri**
- 📡 **Kaynakları**

toplar, birleştirir ve analiz eder.

### 💡 Örnek Senaryo:

**Durum:**
Bir kullanıcı **New York şehir merkezinde** bir bankta oturmuş sandviç yerken, akıllı telefonunda bir oyun oynuyor olsun.

**Hedefleme:**
**Starbucks** (reklamveren), kullanıcının bulunduğu konumdan **5 dakika uzaklıktaki Starbucks şubesine** gitmesini teşvik eden bir reklam gösterebilir.

---

## 💻 Tarayıcı Türü, İşletim Sistemi ve Cihaz Türü
### 🔹 Tanım:

Reklam sunucusuna gönderilen her reklam isteği, bir **User-Agent HTTP header** içerir.

### 📋 Örnek User-Agent:

```
User-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6)
AppleWebKit/537.36 (KHTML, like Gecko)
Chrome/60.0.3112.101 Safari/537.36
```

### 🔍 Bu Örnekten Çıkarılan Bilgiler:

- 💻 **İşletim Sistemi:** Mac OS X 10.12.6
- 🌐 **Tarayıcı:** Chrome
- 📌 **Tarayıcı Sürümü:** 60.0.3112.101

### 📱 Mobil Cihaz Örneği:

Bir başka örnekte, **14D27** kimliği bir **iPhone 7 Plus** cihazını temsil eder ve cihazın **iOS 10.2.1** çalıştırdığı anlaşılır.

### 🎯 Tespit Edilebilen Bilgiler:

Bu bilgiler sayesinde reklam sunucusu:
- 💻 **İşletim sistemini**
- 🌐 **Tarayıcı türünü ve sürümünü**
- 📱 **Cihaz türünü**
- 🏷️ **Marka ve modeli**

tespit edebilir.

### 📱 Mobil Önemi:

Bu özellikle **mobil cihazlar** için oldukça önemlidir (örnekte olduğu gibi iPhone).

---

## 🖥️ Donanım ve Yazılıma Dayalı Hedefleme
### 🔹 Tanım:

Kullanıcıları sahip oldukları **donanım veya yazılım özelliklerine göre** hedeflemek, reklamverenlerin belirli bir kitleye **son derece alakalı mesajlarla** ulaşmasını sağlar.

### 💡 Örnek Senaryo:

**Senaryo:**
Bir mobil oyun şirketi yeni geliştirdiği **Android oyununu** tanıtmak istiyor.

**Hedefleme:**
**Android işletim sistemi** kullanan akıllı telefon ve tablet sahiplerine özel olarak reklam gösterilebilir.

---

## 📚 IAB İçerik Taksonomisi (IAB Content Taxonomy)
### 🔹 Tanım:

**IAB (Interactive Advertising Bureau)**, web sitelerinin kategorize edilmesi için **standart bir taksonomi** sunar.

### 🎯 Kullanım Amaçları:

Reklamverenler:
- ✅ Reklam isteği (ad request) içinde iletilen kategori bilgilerine göre **dijital reklam alanı satın alabilir**
- ❌ Aynı zamanda **belirli kategorilere ait web sitelerinde reklamlarının gösterilmemesini** de tercih edebilir

### 🛡️ Marka Güvenliği:

Bu sayede **marka güvenliği (brand safety)** ve **içerik uyumu** sağlanmış olur.

---

### 📊 IAB İçerik Taksonomisi – Örnek Yapı
Aşağıdaki tablo, **IAB Content Taxonomy'nin hiyerarşik yapısını** (Tier 1 → Tier 2 → Tier 3) örneklerle göstermektedir.

Her satır **benzersiz bir kategori kimliğini (Unique ID)** temsil eder.

| Unique ID | Tier 1                 | Tier 2               | Tier 3                    |
|-----------|------------------------|----------------------|---------------------------|
| 1         | Otomotiv               |                      |                           |
| 2         | Otomotiv               | Araç Kasa Tipi       |                           |
| 3         | Otomotiv               | Araç Kasa Tipi       | Ticari Kamyonlar          |
| ...       | ...                    | ...                  | ...                       |
| 52        | İş ve Finans           |                      |                           |
| 53        | İş ve Finans           | İş Dünyası           |                           |
| 54        | İş ve Finans           | İş Dünyası           | Muhasebe ve Finans        |
| ...       | ...                    | ...                  | ...                       |
| 223       | Sağlıklı Yaşam         |                      |                           |
| 224       | Sağlıklı Yaşam         | Çocuk Sağlığı        |                           |
| 225       | Sağlıklı Yaşam         | Fitness ve Egzersiz  | Katılımcı Sporlar         |
| ...       | ...                    | ...                  | ...                       |
| 239       | Hobiler ve İlgi Alanları|                      |                           |
| 255       | Hobiler ve İlgi Alanları| Sanat ve El İşi      | Fotoğrafçılık             |
| ...       | ...                    | ...                  | ...                       |
| 656       | Seyahat                | Seyahat Lokasyonları | Afrika Seyahati           |
| 657       | Seyahat                | Seyahat Lokasyonları | Asya Seyahati             |
| 658       | Seyahat                | Seyahat Lokasyonları | Avustralya ve Okyanusya   |
| ...       | ...                    | ...                  | ...                       |

---

### 📈 IAB İçerik Taksonomisi Hakkında

**IAB Content Taxonomy:**
- 📊 **30+ adet Tier 1** (üst seviye) kategori
- 📋 **1.100+ adet benzersiz kategori girdisi** içerir

### 🎯 Faydaları:

Bu yapı, içeriklerin **standart ve tutarlı şekilde sınıflandırılmasını** sağlar.

Reklamverenler bu kategorileri kullanarak:
- ✅ **Hangi içeriklerde reklam göstereceklerini**
- ❌ **Hangi içeriklerde reklam göstermeyeceklerini (brand safety)** belirleyebilir

### 📝 Teknik Detay:

Aşağıda gösterilen yapı, **OpenRTB v2.4 spesifikasyonu** içinde yer alan ve **390+ içerik kategorisi** barındıran IAB İçerik Taksonomisinin bir bölümüdür.

---

### 💻 IAB İçerik Kategorileri – Örnekler
Aşağıda, **IAB Content Taxonomy (OpenRTB 2.4)** kapsamında yer alan bazı içerik kategorilerinin örnekleri bulunmaktadır.

Bu kategoriler genellikle **JSON formatında** tanımlanır ve **ad request** içinde kullanılır.

```json
{
  "IAB1": "Sanat ve Eğlence",
  "IAB1-1": "Kitaplar ve Edebiyat",
  "IAB1-2": "Ünlüler / Magazin",
  "IAB1-3": "Güzel Sanatlar",
  "IAB1-4": "Mizah",
  "IAB1-5": "Filmler",
  "IAB1-6": "Müzik",
  "IAB1-7": "Televizyon",

  "IAB2": "Otomotiv",
  "IAB2-1": "Oto Parçaları",
  "IAB2-2": "Araç Tamiri",
  "IAB2-3": "Araç Alım / Satımı",
  "IAB2-4": "Otomobil Kültürü",
  "IAB2-5": "Sertifikalı İkinci El",
  "IAB2-6": "Cabrio",
  "IAB2-7": "Coupe",
  "IAB2-8": "Crossover",
  "IAB2-9": "Dizel",
  "IAB2-10": "Elektrikli Araç",
  "IAB2-11": "Hatchback",
  "IAB2-12": "Hibrit",
  "IAB2-13": "Lüks",
  "IAB2-14": "Minivan",
  "IAB2-15": "Motosikletler",
  "IAB2-16": "Arazi Araçları",
  "IAB2-17": "Performans Araçları",
  "IAB2-18": "Pickup",
  "IAB2-19": "Yol Yardımı",
  "IAB2-20": "Sedan",
  "IAB2-21": "Kamyonlar ve Aksesuarlar",
  "IAB2-22": "Klasik Araçlar",
  "IAB2-23": "Station Wagon",

  "IAB3": "İş Dünyası",
  "IAB3-1": "Reklamcılık",
  "IAB3-2": "Tarım",
  "IAB3-3": "Biyoteknoloji / Biyomedikal",
  "IAB3-4": "İş Yazılımları",
  "IAB3-5": "İnşaat",
  "IAB3-6": "Ormancılık"
}
```

> **📝 Kaynak:** GitHub (IAB OpenRTB 2.4 içerik kategorileri)

---

## 📅 Haftanın Günü ve Günün Saati Hedefleme
### 🔹 Tanım:

Reklamların **haftanın gününe** ve hatta **günün saatine göre** gösterilmesi, reklamverenlerin:
- ✅ **Doğru kitleye doğru zamanda ulaşmasını**
- 💰 **Reklam bütçesinin boşa harcanmasını önlemesini**

sağlar.

---

### 💡 Örnek Senaryo

**Senaryo:**
Büyük bir **pizza restoranı zinciri** için çalışan bir reklamveren

**Hedefleme:**
**Cuma akşamı kampanyalarını** Cuma günleri **15:00 – 20:00** saatleri arasında yayınlamayı tercih edebilir.

### 🎯 Stratejik Avantajlar:

Bu strateji özellikle:
- ⚡ **Aynı saatlerde rakiplerin özel bir kampanya sunmadığı durumlarda**
- 🎯 **Reklamın rakip içeriklerin yanında gösterildiği senaryolarda**

çok daha etkili olur.

---

### 📈 Performans Odaklı Zamanlama

**Durum:**
Bir marka reklam etkileşiminin **günün belirli saatlerinde daha yüksek** olduğunu fark ederse

**Strateji:**
Reklamlarını bu zaman aralıklarında göstermeyi seçebilir.

### ✅ Sonuçlar:

Bu sayede:
- 📈 **Hedef kitleye ulaşma olasılığı artar**
- 🎯 **Etkileşim oranları yükselir**
- 📊 **Tıklama oranları (CTR) ve dönüşümler artar**

---

## 🧠 Davranışsal Hedefleme (Behavioral Targeting)
### 🔹 Tanım:

**Davranışsal hedefleme**, **çevrimiçi davranışsal reklamcılık (Online Behavioral Advertising – OBA)** olarak da bilinir.

### 📋 Açıklama:

Bu yöntem, reklamverenlerin ve yayıncıların, kullanıcıların **web üzerindeki gezinme davranışlarına dayanarak** onlara ilgili reklamlar ve pazarlama mesajları göstermesine olanak tanır.

---

### 📊 Davranışsal Hedefleme için Toplanan Veri Türleri:

Davranışsal hedefleme için toplanan veri türlerine şunlar dahildir:
- 📄 **Ziyaret edilen sayfalar**
- 🔍 **Önceki arama terimleri**
- ⏱️ **Bir web sitesinde geçirilen süre**
- 🖱️ **Tıklanan reklamlar ve butonlar**
- 📥 **Görüntülenen ve indirilen içerikler**
- 🛒 **Yapılan satın almalar**
- 📅 **Son web sitesi ziyaretinin tarihi**
- 🔗 **Kullanıcıların farklı web siteleriyle olan etkileşimlerine dair diğer bilgiler**

---

### 🔄 Çevrimiçi Davranışsal Hedefleme Süreci

**Süreç Akışı:**

1. 👤 **Kullanıcı** bir web sitesini ziyaret eder
2. 📡 **Reklam Alanı (Ad slot)** reklam isteği gönderir
3. 🖥️ **Yayıncının Reklam Sunucusu** veriyi işler
4. 🔄 **Reklam Borsası (Ad exchange)** ve **SSP** veriyi alır
5. 📊 **DMP (Data Management Platform)** kullanıcı hakkında bilgileri sağlar:
   - 🍪 Çerez bilgisi (cookie)
   - 👥 Demografik bilgiler
   - 📈 Davranışsal profil
   - 📜 Tarama (gezinme) geçmişi
6. 💰 **DSP (Demand-Side Platform)** teklif verir
7. 👁️ **Reklam kullanıcıya gösterilir**

> **💡 Not:** Çevrimiçi davranışsal hedefleme, hangi reklamların gösterileceğini belirlemek için **kullanıcıya ait bilgileri** kullanır.

---

## ⚙️ Davranışsal Hedefleme Süreci

Davranışsal hedefleme süreci **üç ana adımdan** oluşur:

### 📋 Genel Süreç:

1. 👤 Kullanıcı bir web sitesini ziyaret eder ve bu ziyaret sırasında kullanıcıya ait veriler (çerezler, gezinme geçmişi vb.) toplanır.
2. 🔄 Bu veriler, yayıncının reklam sunucusu üzerinden **Ad Exchange**, **SSP** ve **DMP** gibi AdTech platformlarına iletilir.
3. 💰 **DSP'ler**, kullanıcı profiline en uygun reklamlar için teklif verir ve kazanan reklam kullanıcıya gösterilir.

---

### 1️⃣ Veri Toplama (Data Collection)
#### 🔹 Tanım:

Reklamverenler, yayıncılar ve **DMP'ler (Data Management Platform)**, kullanıcıların farklı web siteleri ve uygulamalar boyunca gerçekleştirdiği aksiyonlara dair veriler toplar.

#### 📊 Event Data:

Bu veriler genellikle **Event Data** olarak adlandırılır ve şunları kapsar:
- 📄 **Sayfa görüntülemeleri**
- 🛍️ **Ürün görüntülemeleri**
- 🛒 **Satın alınan ürünler**
- 🔗 **Bir web sitesi veya mobil uygulamadaki diğer etkileşimler**

#### 🔗 Veri Bağlama:

Bu veriler daha sonra:
- 🍪 **Web tarayıcılarında bulunan birinci taraf (first-party) ve üçüncü taraf (third-party) çerezlerde** saklanan tanımlayıcılar
- 📱 **Mobil uygulamalarda kullanılan mobil cihaz kimlikleri (mobile IDs)**

aracılığıyla birbirine bağlanır.

#### 👤 Kullanıcı Profilleri:

Ardından, belirli bir kullanıcıya ait tüm **Event Data**’yı tek bir yerde tutmak için **kullanıcı profilleri** oluşturulur ve gelecekteki tüm **Event Data** bu profile atanır.

#### 🔑 Tanımlayıcılar:

Üçüncü taraf çerezlerdeki bir ID ya da mobil cihaz kimliği gibi bir tanımlayıcı, kullanıcıyı farklı web sitelerindeki aksiyonlarıyla ilişkilendirmek ve **Event Data**’yı doğru kullanıcı profiline bağlamak için kullanılır.

---

### 2️⃣ Kitle Oluşturma (Audience Creation)
#### 🔹 Tanım:

Reklamverenler ve yayıncılar, bireysel kullanıcı profillerinden oluşan **kitleler (audiences)** oluşturur.

#### 💡 Örnek Kriterler:

Örneğin bir reklamveren, aşağıdaki kriterleri karşılayan kullanıcıları içeren bir kitle oluşturabilir:
- 🛍️ **Belirli bir ürünü bir ay içinde üçten fazla kez görüntülemiş olanlar**
- 📧 **Bir bültene (newsletter) kayıt olmuş olanlar**
- 🔄 **Son 60 gün içinde web sitesini en az 15 kez ziyaret etmiş olanlar**

---

### 3️⃣ Verinin Uygulanması (Application of Data)
#### 🔹 Tanım:

Reklamveren, oluşturulan bu kitleleri **çevrimiçi medya kampanyalarında reklam hedefleme amacıyla** kullanır.

#### ✅ Sonuçlar:

Bunun sonucunda:
- 🎯 **Kullanıcılara gösterilen reklamlar daha alakalı (relevant) hale gelir**
- 📈 **Kullanıcıların dönüşüm gerçekleştirme (ör. ürün satın alma) olasılığı artar**

---

### 📊 Davranışsal Hedefleme Sürecinin 3 Temel Adımı

1. 📥 **Verilerin toplanması ve analiz edilmesi**
2. 👥 **Segmentasyon (kitlelere ayırma)**
3. 🎯 **Verinin uygulanması (reklam hedefleme)**

Davranışsal hedefleme süreci bu üç temel adımdan oluşur.

---

## 🔄 Yeniden Hedefleme (Retargeting)

### 🔹 Tanım:

**Yeniden hedefleme (Retargeting)**, markayla **daha önce etkileşime geçmiş kullanıcılara** reklam gösterilmesidir.

### ⚙️ Nasıl Çalışır?

#### 📋 Adım Adım Süreç:

1. 📍 **Tracking Pixel Yerleştirme:**
   - Siteye **1x1 tracking pixel** yerleştirilir

2. 🍪 **Cookie Oluşturma:**
   - Kullanıcı pixel'i tetikler → **cookie oluşturulur**

3. 🔍 **Kullanıcı Tanıma:**
   - Kullanıcı başka bir siteye gittiğinde **tanınır**

4. 👁️ **Reklam Gösterimi:**
   - **Önceden görüntülediği ürün** reklam olarak gösterilir

## 🎓 Bölüm Özeti

Bu bölümde Hedefleme ve Bütçe Kontrolü konularının temellerini öğrendik:

### **📚 Öğrendiklerimiz:**

1. **🎯 Hedefleme Tanımı** - Belirli kriterlere uyan kullanıcılara reklam gösterme
2. **🌐 Bağlamsal Hedefleme** - İçerik tabanlı hedefleme yöntemi
3. **🔑 Anahtar Kelimeler** - İçerik analizi ve hedefleme
4. **📍 Reklam Pozisyonu** - Boyut ve konum bazlı hedefleme
5. **🌍 Coğrafi Hedefleme** - IP ve GPS tabanlı konum belirleme
6. **💻 Cihaz ve Tarayıcı Hedefleme** - User-Agent bazlı tespit
7. **📚 IAB İçerik Taksonomisi** - Standart içerik kategorileri
8. **📅 Zaman Bazlı Hedefleme** - Gün ve saat bazlı gösterim
9. **🧠 Davranışsal Hedefleme** - Kullanıcı davranışına dayalı hedefleme
10. **🔄 Yeniden Hedefleme** - Önceki etkileşimlere dayalı reklam gösterimi

### **🔑 Ana Çıkarımlar:**

- **Çeşitlilik:** Farklı hedefleme yöntemleri farklı amaçlara hizmet eder
- **Gizlilik:** Bağlamsal hedefleme kişisel veri gerektirmez
- **Verimlilik:** Doğru hedefleme ROI'yi artırır
- **Uyumluluk:** GDPR ve benzeri regülasyonlara uyum sağlar

---

[⬅️ Bölüm 06: Ad Serving (Reklam Sunucuları)](/The-AdTech-Book/bolumler/06-ad-serving.md) | [🏠 Ana Sayfa](/The-AdTech-Book/index.md) | [➡️ Bölüm 08: İzlenim, Tıklama ve Dönüşüm Takibi](/The-AdTech-Book/bolumler/08-izlenim-tiklama-donusum-takibi.md)
