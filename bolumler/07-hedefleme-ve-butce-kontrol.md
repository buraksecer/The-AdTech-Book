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

## 🎓 Bölüm Özeti

Bu bölümde Hedefleme ve Bütçe Kontrolü konularının temellerini öğrendik:

### **📚 Öğrendiklerimiz:**

1. **🎯 Hedefleme Tanımı** - Belirli kriterlere uyan kullanıcılara reklam gösterme
2. **🌐 Bağlamsal Hedefleme** - İçerik tabanlı hedefleme yöntemi
3. **🔑 Anahtar Kelimeler** - İçerik analizi ve hedefleme
4. **📍 Reklam Pozisyonu** - Boyut ve konum bazlı hedefleme
5. **🌍 Coğrafi Hedefleme** - IP tabanlı konum belirleme

### **🔑 Ana Çıkarımlar:**

- **Çeşitlilik:** Farklı hedefleme yöntemleri farklı amaçlara hizmet eder
- **Gizlilik:** Bağlamsal hedefleme kişisel veri gerektirmez
- **Verimlilik:** Doğru hedefleme ROI'yi artırır
- **Uyumluluk:** GDPR ve benzeri regülasyonlara uyum sağlar

### **📈 Sonraki Bölümlerde:**

- İzlenim, tıklama ve dönüşüm takibi
- Bütçe kontrolü mekanizmaları
- Frequency capping (Frekans sınırlaması)
- Davranışsal hedefleme
- Demografik hedefleme

---

[⬅️ Bölüm 06: Ad Serving (Reklam Sunucuları)](06-ad-serving.md) | [🏠 Ana Sayfa](../index.md) | [➡️ Bölüm 08: İzlenim, Tıklama ve Dönüşüm Takibi](08-izlenim-tiklama-ve-donusum-takibi.md)
