# 📊 SWOT Analizi — Yılmaz Makina YILPAK DPC 500
**Tarih:** 15 Kasım 2026  
**Hazırlayan:** Samet Yeşilot (Öğr. No: 230541036 · @sametyesilot)  
**Makine:** Yılmaz Makina — YILPAK DPC 500 Tam Otomatik Dikey Paketleme ve Dolum Makinesi (SAMİB Üyesi)  
**Kapsam:** Safety 4.0 & Cyber-Physical Systems (LAB 1–7 Föyleri Analizi)  

---

## 📌 Genel Değerlendirme

Yılmaz Makina YILPAK DPC 500, dakikada 180–190 paket kapasitesine ulaşabilen yüksek hızlı servo kontrollü dikey paketleme (VFFS) mimarisiyle üretim verimliliğinde güçlü bir avantaj sunar; en büyük açığı, uzaktan bakım/servis ve hat entegrasyonu kaynaklı siber-emniyet riskidir. Asıl strateji, ısıl yapıştırma çenesi, kesim bıçağı ve kapak kilitleme gibi emniyet fonksiyonlarını dijital ağdan tamamen izole ederek bu riski kapatmak ve bunu ölçülebilir bir güven avantajına dönüştürmektir.

*Analiz, makinenin resmi teknik parametreleri (400 VAC / 5 kW, 6 bar pnömatik, 180–190 paket/dk, maks. 600 mm OPP/CPP/PET/AL-PE bobin) ile makine üzerinde doldurduğumuz LAB 1–7 föylerine dayanır; gerçek saha olay veya üretim logları içermez.*

---

## 🧭 SWOT Matrisi

### 🏢 İç Faktörler

| Güçlü Yönler (Strengths - S) | Zayıf Yönler (Weaknesses - W) |
| :--- | :--- |
| • **Yüksek paketleme hızı ve esneklik:** 180–190 paket/dk kapasite; OPP, CPP, PET ve AL-PE filmlerle yüksek hat verimliliği. | • **Uzak erişim dijital kesişim noktası:** Yanlış yapılandırılırsa uzaktan servis modülü Safety PLC konfigürasyonuna ulaşabilir. |
| • **Kompakt ve enerji verimli yapı:** 5 kW / 400 VAC güç ve 6 bar pnömatik altyapı ile düşük işletme maliyeti. | • **Paylaşılan servis hesabı riski:** Sürekli açık uzak erişim, port 80 HMI ve eksik oturum kaydı açıklığı. |
| • **Ayrı safety yolu:** E-stop, kapak kilidi ve yükleme bölgesi ışık perdesi $\to$ Safety PLC $\to$ STO + pnömatik tahliye ile insan korunması. | • **PLC firmware kütüphane zafiyetleri:** Üçüncü taraf bileşen açıkları (örn. Component X 2.4) ve yama sonrası safety yeniden validasyon yükü. |
| • **Hızlı uzaktan teşhis ve servis:** Uzaktan reçete/servo parametre kontrolüyle düşük duruş süresi. | • **YZ kalite kontrol kırılganlığı:** Kamera tabanlı mühür/baskı kontrolünde yanlış sınıflandırma ve manipüle edilmiş görüntü riski. |
| • **Savunulabilir zone/conduit mimarisi:** Z1–Z5 katmanlı izolasyonla safety ve üretim ağının ayrılması. | • **Doğuştan fiziksel tehlikeler:** Yüksek sıcaklıktaki ısıl yapıştırma çeneleri, pnömatik kesim bıçağı ve 600 mm bobin tahriki. |

---

### 🌐 Dış Faktörler

| Fırsatlar (Opportunities - O) | Tehditler (Threats - T) |
| :--- | :--- |
| • **Siber güvenlik ve emniyet kanıtı:** Evidence Pack (EP 02–15) büyük gıda/kimya müşterilerinin ihalelerinde fark yaratır. | • **Yetkisiz erişim ve manipülasyon:** Çalınmış servis hesabıyla çene sıcaklığı, basınç veya kapak kilidi gecikmesinin değiştirilmesi. |
| • **Akıllı fabrika (Industry 4.0) talebi:** OEE, fire ve mühür kalitesi verisinin MES/ERP'ye güvenli tek yönlü aktarımı. | • **Üretim ve hat durması:** Fidye yazılımı (ransomware) veya ofis ağından yayılan saldırılarla paketleme hattının kilitlenmesi. |
| • **Tahmine dayalı bakım hizmeti:** Çene rezistansı, bıçak aşınması ve pnömatik kaçak izleme ile ek servis geliri. | • **Tedarik zinciri zafiyetleri:** PLC/HMI üçüncü taraf kütüphanelerinde kritik CVE'ler ve SBOM eksikliği. |
| • **Mevzuata erken hazırlık:** AB CRA (Cyber Resilience Act) ve Makine Tüzüğü (EU 2023/1230) erken uyum avantajı. | • **Yasal yaptırımlar:** 24 saat / 72 saat / 14 gün olay bildirim yükümlülüklerine uyulmaması sonucu cezalar. |
| • **Sürdürülebilirlik ve sıfır fire:** YZ tabanlı erken sızdırmazlık/hizalama tespitiyle film ve ürün firesinin azaltılması. | • **Pazar rekabeti:** Rakiplerin varsayılan güvenli (secure-by-design) akıllı VFFS makineleriyle pazara girmesi. |

---

## 🎯 Stratejik Çıkarımlar

| Strateji Türü | Tanım | Eylem ve Uygulama |
| :--- | :--- | :--- |
| **SO (Güçlüyü Fırsatla Büyüt)** | Güçlü yönleri fırsatlarla eşleştirme | Ayrı safety mimarisini ve Evidence Pack dokümantasyonunu satış argümanı yap; *"Çene ve bıçak güvenliği ağdan bağımsız"* mesajıyla kurumsal müşterilere ulaş. |
| **WO (Zayıfı Fırsatla Kapat)** | Zayıf yönleri fırsatlarla iyileştirme | Uzak erişimi Jump Server + VPN + MFA + kişisel hesap + tam oturum kaydı + varsayılan kapalı modeline taşı; kestirimci bakım servisini bu güvenli kanal üzerinden sun. |
| **ST (Güçlüyü Tehditle Koru)** | Güçlü yönlerle tehditlere kalkan olma | Safety zone'u normal PLC ve uzak erişimden izole tut; saldırgan HMI/Üretim PLC'ye girse bile STO ve pnömatik boşaltmanın donanımsal çalışmasını düzenli test et. |
| **WT (Zayıf ve Tehdit Birleşimini Önle)** | Savunma ve kriz yönetimi | Canlı SBOM tut, kritik CVE'leri test tezgâhında doğrula; YZ kalite modülüne güven eşiği ve fallback ekle; 24s / 72s / 14 gün CRA olay tatbikatını prova et. |

---

## 🚀 İlk 5 Öncelikli Eylem

1. [ ] **Uzak erişim sertleştirme:** Paylaşılan `admin/admin` hesabını kaldır; VPN + MFA + Jump Server + kişisel hesap + tam oturum kaydına geç.
2. [ ] **Safety izolasyonu:** Safety PLC'yi ayrı Z1 bölgesine al; program/parametre yüklemeyi yalnızca yerel ve fiziksel anahtarlı yap.
3. [ ] **SBOM & CVE süreci:** YILPAK DPC 500 PLC/HMI SBOM'unu oluştur; Component X 2.4 için üç şartı (bileşen, sürüm, ulaşılabilirlik) doğrula.
4. [ ] **Çene & Bıçak Emniyeti Doğrulaması:** Kapak kilidi (guard locking) ve ışık perdesi tepki/durma süresini çene soğuma/geri çekilme ile birlikte düzenli test et.
5. [ ] **YZ Fail-Safe kurgusu:** Kamera tabanlı mühür/baskı kontrolünde güven eşiği (%90 / %70–90 / <%70), çapraz fotosel doğrulaması ve güvenli fallback tanımla.

---
*Çıktı Belgesi: Evidence Pack EP 02, EP 03, EP 04, EP 05, EP 09, EP 13, EP 15 Stratejik Değerlendirme Özeti.*
