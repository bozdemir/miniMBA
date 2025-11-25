# Finansal Yönetim Dersi - Kapsamlı Rapor

## 1. Ders Özeti

Bu rapor, finansal yönetim dersinin ilk bölümünü oluşturan sesli ve görsel materyallerden derlenen temel finansal kavramları ve analizleri sunmaktadır. Faiz kavramının tarihsel ve etik boyutlarından başlayarak, basit ve bileşik faiz hesaplamaları, reel faiz ve anüite gibi finansal matematik konuları detaylandırılmıştır. Excel'in bu hesaplamalardaki pratik kullanımı gösterilmiş, Türkiye ekonomisine özgü enflasyon, kur riski ve konut piyasası gibi güncel finansal konulara değinilmiştir. Rapor, finansal kararlar alırken risk faktörlerini ve piyasadaki aldatmacaları anlamanın kritik önemini vurgulamaktadır.

## 2. Alt Başlıklar

### 2.1. Faiz Kavramı ve Bileşenleri

*   **Faiz Tanımı:** Faiz, "paranın kirası" veya "paranın maliyeti" olarak tanımlanır.
*   **Tarihsel ve Etik Perspektifler:** Antik Yunan'dan (sömürü, risk/emek eksikliği nedeniyle etik dışı) tek tanrılı dinlere (haram) kadar faize yönelik farklı bakış açıları incelenmiştir. Kağıt paraya (fiat money) geçişin faiz algısını ve gerekçelendirmesini değiştirdiği belirtilmiştir.
*   **Tefecilik:** Ekonomik kriz dönemlerinde bankaların kredi vermekten çekinmesiyle tefeciliğin arttığı, sömürücü bir uygulama olduğu ve acımasızca yüksek faizlerle çalıştığı vurgulanmıştır. Tefecilerin genellikle bankacılığa karşı olduğu ve faizin haram olduğunu söyleseler de kendilerinin en yüksek faizi aldıkları belirtilmiştir.
*   **Faiz Oranının Bileşenleri:** Faiz oranı, aşağıdaki unsurlardan oluşur:
    *   Paranın zaman değeri
    *   Enflasyon risk primi
    *   Geri ödeyememe risk primi (default risk)
    *   Likidite risk primi (Paraya çevirememe riski)
    *   Vade risk primi
    *   Kar risk primi (Görselde belirtilmiştir, sesli anlatımda diğer risklerle birlikte ele alınmıştır.)
*   **Paranın Zaman Değeri (Fırsat Maliyeti):** Diğer riskler olmasa bile, paranın alternatif yatırım araçlarında kazanabileceği getiri (fırsat maliyeti) nedeniyle bir zaman değeri olduğu ve faizin temelini oluşturduğu belirtilmiştir. Faizin yasaklanmasının para akışını durduracağı ve borç vermeyi engelleyeceği savunulmuştur.
*   **Likidite Kavramı:** Bir varlığın değer kaybetmeden hızla nakde çevrilebilme yeteneği olarak açıklanmış, örneklerle (ikinci el araba piyasası, Hazine kağıtları) somutlaştırılmıştır. Hazine kağıtlarının Borsa İstanbul'da yüksek işlem hacmi nedeniyle likit olduğu belirtilmiştir.
*   **Vade Riski:** Vade uzadıkça belirsizliğin arttığı ve genellikle daha yüksek faiz gerektirdiği, ancak Türkiye piyasasında bunun tersi durumların da görülebildiği (verim eğrisi) belirtilmiştir.
*   **Kur Riski:** Türk Lirası'nın nominal değer kaybına rağmen, dezenflasyon programıyla reel anlamda değer kazanmaya başladığı, ancak bunun emek yoğun sektörlerde iş kaybına (örn. tekstil sektöründe 350.000 iş kaybı) yol açtığı ve kur riskinin hala mevcut olduğu ifade edilmiştir.

### 2.2. Faiz Hesaplamaları ve Excel Kullanımı

*   **Basit Faiz:**
    *   Formülü: FV = PV * (1 + i * n). (Görselde: FV:GB CV:BD, PV=100TL, i=%10, n=2yıl. FV = 100(1+0,1x2) = 120TL)
    *   Gerçek hayatta fiilen kullanılmadığı, sadece bir yıldan kısa vadeli Hazine bonosu gibi istisnai durumlarda kullanıldığı belirtilmiştir.
    *   "Nominal faiz", bir yıllık basit faiz oranı olarak tanımlanmıştır. Bankaların mevduatta yıllık, kredide ise aylık nominal faiz oranları kullanarak yanıltıcı olabileceği vurgulanmıştır.
*   **Bileşik Faiz:**
    *   Formülü: FV = PV * (1 + i)^n. (Görselde: FV=PV(1+i)ⁿ 100(1+0,1)² =121 TL.)
    *   Gerçek hayattaki finansal işlemlerde kullanılan yöntemdir. Faizden faiz kazanma prensibine dayanır.
    *   "Efektif faiz" (veya Etkin faiz), bir yıllık bileşik faiz oranı olarak tanımlanmıştır.
*   **Temel Parametreler:** Gelecekteki Değer (FV), Bugünkü Değer (PV), Faiz Oranı (i/RATE), Dönem Sayısı (n/NPER) olmak üzere dört ana parametre bulunur. Bu parametrelerden biri sorulduğunda diğer üçünün verilmesi gerekir.
*   **Excel Fonksiyonları:**
    *   **FV (Future Value):** Gelecekteki değeri hesaplamak için kullanılır. (Örnek: 150.000 TL %42 3yıl = 429.493,20 TL)
    *   **PV (Present Value):** Bugünkü değeri hesaplamak için kullanılır.
    *   **RATE:** Faiz oranını hesaplamak için kullanılır. (Formülü: i = (FV/PV)^(1/n) - 1)
    *   **NPER:** Dönem sayısını hesaplamak için kullanılır. (Formülü: n = ln(FV/PV) / ln(1+i))
    *   **Kullanım Notları:** Excel'de nakit giriş ve çıkışlarının ters işaretli girilmesi gerektiği, parametrelerin (faiz oranı ve dönem sayısı) uyumlu olması gerektiği (örn. aylık faiz için aylık dönem sayısı) vurgulanmıştır.
*   **Efektif Yıllık Faiz Oranı (EAR) Hesaplaması:**
    *   Formülü: Rf = (1 + R_nom / M)^M - 1. (Görselde: Rf = (1 + r_nom / m)^m - 1)
    *   Farklı bileşikleştirme sıklıklarına sahip yatırım seçeneklerini karşılaştırmak ve en avantajlı olanı belirlemek için kullanılır. M, bir yılda faizden kaç kere faiz kazanıldığını gösteren indirgeme katsayısıdır (örn. günlük repo için 365, aylık için 12).
    *   Örnek tablo (Görselden):
        | Hesap Türü | Nominal Faiz (R_nom) | M (İndirgeme Katsayısı) |
        | :--------- | :------------------- | :---------------------- |
        | Günlük Repo | 0.15                 | 365                     |
        | 1 Aylık     | 0.38                 | 12                      |
        | 3 Aylık     | 0.40                 | 4                       |
        | 6 Aylık     | 0.42                 | 2                       |
        | 1 Yıllık    | 0.43                 | 1                       |
*   **Sürekli Bileşikleştirme:** Teorik bir limit olarak tanıtılmış, Euler sayısı (e = 2.718282) kullanılarak hesaplanır (ref = e^r - 1). Gerçek hayatta pratik bir kullanımı olmadığı, ancak düşük faiz oranlarında kesikli bileşikleştirme ile farkın az olduğu belirtilmiştir.

### 2.3. Reel Faiz ve Ekonomik Analizler

*   **Reel Faiz Tanımı:** Enflasyondan arındırılmış faizdir. İçerisinde paranın zaman değeri, likidite riski, kur riski, geri ödeyememe riski ve vade riski gibi beş bileşen bulunur. (Görselde: Reel faiz = Enflasyondan arındırılmış)
*   **Reel Faiz Hesaplaması (Türkiye için):** Türkiye gibi yüksek enflasyonlu ülkelerde, nominal faiz oranından gelecekteki enflasyon beklentisinin çıkarılmasıyla hesaplanır. Merkez Bankası'nın geleceğe yönelik enflasyon öngörüleri bu hesaplamada kritik öneme sahiptir. (Görselde: = (1 + 0.40 faiz oranı - 1) / (1 + 0.16) - bu formül reel faiz hesaplamasının bir örneğidir, ancak eksik görünmektedir. Doğru formül (1+nominal faiz)/(1+enflasyon oranı) - 1 şeklindedir.)
*   **Merkez Bankası Enflasyon Beklentileri:** Merkez Bankası'nın beklenti anketlerinde hane halkı beklentisi en yüksek, piyasa beklentisi en düşük, reel sektör beklentisi ise genellikle gerçek enflasyonu en iyi yansıtan olarak kabul edilir. Merkez Bankası'nın enflasyon tahminlerinin aralık tahmini şeklinde sunulduğu ve belirsizlik içerdiği (örn. %12-20 arası %70 ihtimal) vurgulanmıştır.
*   **Merkez Bankası'nın Zorlukları:** Türkiye'de sadece TL değil, dolar, euro, altın gibi farklı para birimlerinin de kullanılması nedeniyle Merkez Bankası'nın para politikası uygulamasının zor olduğu ifade edilmiştir.
*   **Yüksek Faiz Oranlarının Etkisi:** Yüksek faiz oranlarının "paradan para kazanmayı" (rantiyecilik) cazip hale getirdiği, girişimciliği ve üretimi engellediği, 2001 krizi gibi dönemlerde bunun olumsuz etkilerinin görüldüğü belirtilmiştir.

### 2.4. Anüite Kavramı ve Uygulamaları

*   **Anüite Tanımı:** Düzenli, eşit ödemelerle gelecekteki birikimi veya bugünkü değeri hesaplamak için kullanılan finansal bir araçtır (devresel ödeme, eşit ödeme). (Görselde: Anuit, Pmt -> Devresel Ödeme)
*   **Anüite Parametreleri:** Gelecekteki Değer (FV), Bugünkü Değer (PV), Düzenli Ödeme Miktarı (A/PMT), Faiz Oranı (i/RATE), Dönem Sayısı (n/NPER) olmak üzere beş parametre bulunur. Bir tanesi sorulduğunda diğer üçünün verilmesi gerekir. (Görselde: Anuite hesaplama 5 parametreden (FV,PV) 2 parametre 3 parametre verilmesi zorunda. A, i, n: 3 parametre.)
*   **Dönem Başı/Dönem Sonu Anüite:** Ödemelerin dönemin başında mı yoksa sonunda mı yapıldığı, hesaplama sonucunu etkiler. Excel'de `Type` parametresi ile belirtilir (0 veya boş: dönem sonu; 1: dönem başı).
*   **Excel PMT Fonksiyonu:** Düzenli ödeme miktarını hesaplamak için kullanılır.
*   **Uygulama Alanları:**
    *   **Çocuk Eğitimi İçin Birikim:** Düzenli Euro yatırımlarıyla çocuğun yurt dışında eğitim masraflarını karşılamak gibi birikim hedefleri için anüite hesaplamaları kullanılmıştır. (Örnek: A = 200 €, i = 0.04/12, n = 216 dönem için FV hesaplaması)
    *   **Bireysel Emeklilik Sistemleri (BES):** BES'te sunulan getirilerin "bugünkü değeri"nin sorgulanması gerektiği, enflasyonun paranın değerini erittiği ve geçmişte sigorta şirketlerinin bu durumdan faydalandığı örneklerle açıklanmıştır.
    *   **Konut Kredileri ve Fiyat Değerlemesi:** Konut alımında ödenen taksitlerin (PMT) veya konutun bugünkü değerinin (PV) hesaplanmasında anüite prensipleri kullanılır. Konut fiyatlarının makul olup olmadığını anlamak için kira çarpanı (örn. 20 yıllık kira) gibi basit yöntemler önerilmiştir. Konut alırken en az bir yıl araştırma yapılması gerektiği belirtilmiştir.
*   **İstanbul Finans Merkezi:** İstanbul'un küresel finans merkezi olma hedefinin sadece bina yapmakla değil, ekonomik istikrar, yaşanabilirlik ve kaliteli finansal eğitim kurumlarıyla mümkün olabileceği belirtilmiştir.
*   **Finansal Okuryazarlık:** Finans alanında "sahtekar gibi düşünmek" ve piyasadaki aldatmacaları anlamak için hesap kitap yapmanın önemi vurgulanmıştır.

## 3. Eylem Maddeleri

1.  Finansal kararlar alırken faiz oranlarının sadece nominal değerlerine değil, paranın zaman değeri, enflasyon, likidite, vade ve kur riskleri gibi tüm bileşenlerine dikkat edilmelidir.
2.  Merkez Bankası'nın faiz indirimleri gibi politikalarının piyasa üzerindeki potansiyel olumsuz etkileri (örn. dolarizasyon) göz önünde bulundurulmalıdır.
3.  Yatırım kararları verilirken, özellikle yüksek enflasyonlu ortamlarda, sunulan getirilerin "bugünkü değeri" sorgulanmalı ve paranın zaman içindeki değer kaybı hesaba katılmalıdır.
4.  Farklı vadeli mevduat veya yatırım seçenekleri karşılaştırılırken, efektif yıllık faiz oranları (EAR) hesaplanarak gerçek getiri potansiyeli belirlenmelidir.
5.  Konut alımı gibi büyük yatırımlarda, piyasadaki standart eksikliği nedeniyle en az bir yıl detaylı araştırma yapılmalı ve konutun makul değeri kira çarpanı gibi yöntemlerle değerlendirilmelidir.
6.  Bireysel emeklilik sistemleri gibi uzun vadeli birikim araçlarında, gelecekteki birikim miktarının bugünkü karşılığı (present value) mutlaka sorgulanmalıdır.
7.  Finansal piyasalardaki "aldatmacaları" anlamak ve doğru kararlar verebilmek için finansal okuryazarlık ve hesaplama becerileri geliştirilmelidir.
8.  Excel gibi araçlar kullanılarak finansal hesaplamalar (FV, PV, RATE, NPER, PMT) doğru bir şekilde yapılmalı, özellikle parametre uyumu (örn. aylık faiz ve dönem sayısı) ve işaret kurallarına dikkat edilmelidir.
9.  Ekonomik kriz dönemlerinde tefecilik gibi sömürücü uygulamalardan kaçınılmalı ve bankaların kredi verme eğilimleri takip edilmelidir.
10. Türkiye ekonomisindeki enflasyon, kur ve faiz dinamikleri yakından takip edilmeli, Merkez Bankası'nın beklentileri reel sektör beklentileriyle karşılaştırılarak daha gerçekçi öngörüler elde edilmeye çalışılmalıdır.
