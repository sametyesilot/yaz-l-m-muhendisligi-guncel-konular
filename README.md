# 📦 Yazılım Mühendisliğinde Güncel Konular
## Safety 4.0: Siber-Fiziksel Sistemler, Fonksiyonel Emniyet & Endüstriyel Siber Güvenlik

![Safety 4.0](https://img.shields.io/badge/Safety_4.0-Bootcamp-0052cc?style=for-the-badge&logo=shield)
![Standard](https://img.shields.io/badge/IEC_62443-Security_Level_3%2F4-brightgreen?style=for-the-badge)
![Functional Safety](https://img.shields.io/badge/ISO_13849--1-PL_e_%7C_SIL_3-red?style=for-the-badge)
![Machine](https://img.shields.io/badge/Machine-Yilmaz_Makina_YILPAK_DPC_500-orange?style=for-the-badge)
![Member](https://img.shields.io/badge/SAM%C4%B0B-%C3%9Cyesi-1f6feb?style=for-the-badge)

Bu depo, **Yazılım Mühendisliğinde Güncel Konular** dersi kapsamında yürütülen **Safety 4.0 Bootcamp** laboratuvar çalışmalarını içermektedir. Proje makinesi, **SAMİB (Sakarya Makina İmalatçıları Birliği)** üyesi **Yılmaz Makina San. ve Tic. Ltd. Şti.** tarafından üretilen **YILPAK DPC 500 Tam Otomatik Dikey Paketleme ve Dolum Makinesi** olarak seçilmiştir. Çalışmalar iki ana klasör ve bir stratejik SWOT analizi altında toplanmıştır:

* **[`2.1 şişeleme föyleri/`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri):** 2.1 Genel Sürüm şablonunun **kendi makinemiz olan Yılmaz Makina YILPAK DPC 500** için uyarlanmış 1'den 7'ye kadar tüm laboratuvar föyleri (`.pdf`).
* **[`2.2 paketleme föyleri/`](./2.2%20paketleme%20f%C3%B6yleri):** 2.2 Paketleme Makinesi şablonunun **kendi makinemiz olan Yılmaz Makina YILPAK DPC 500 (Tam Otomatik Dikey Paketleme ve Dolum Makinesi)** için 1'den 7'ye kadar eksiksiz uyarlanmış görsel PDF çıktıları.

---

## 🏭 Kendi Makinemiz: Yılmaz Makina — YILPAK DPC 500

| Parametre | Açıklama |
| :--- | :--- |
| **Üretici / Kuruluş** | **Yılmaz Makina San. ve Tic. Ltd. Şti.** — **SAMİB Üyesi** ([samib.org.tr](https://samib.org.tr/uye/yilmaz-makina-san-ve-tic-ltd-sti/)) |
| **Model** | **YILPAK DPC 500 (Tam Otomatik Dikey Paketleme ve Dolum Makinesi)** |
| **Makine Tipi** | Endüstriyel Dikey Form-Doldur-Kapat (VFFS) Paketleme Sistemi |
| **Uygulama Alanı** | Tanecikli ve granül ürünler (bakliyat, kuruyemiş, deterjan, şeker, tuz, kimyasal granüller) |
| **Paketleme Kapasitesi** | Maksimum **180 – 190 adet/dakika** (film genişliği, paket boyu ve ürün yoğunluğuna bağlı) |
| **Boyutlar & Ağırlık** | **1280 mm (G) × 2370 mm (U) × 1700 mm (Y)** · **1050 kg** gövde ağırlığı |
| **Güç & Pnömatik** | **400 VAC · 5 kW** elektrik tahriki · **6 bar** pnömatik hava basıncı |
| **Bobin & Film Özellikleri** | Maks. **600 mm** bobin dış çapı · **OPP, CPP, PET, AL-PE** ve laminasyonlu filmler |
| **Tahrik & Tehlikeli Üniteler** | Servo kontrollü film çekme kayışları, yüksek sıcaklıkta yatay/dikey ısıl yapıştırma çeneleri ve pnömatik kesim bıçağı |
| **Otomasyon Altyapısı** | Safety PLC (SIL 3 / PL e) + Üretim PLC'si + Dokunmatik HMI + Uzak Bakım Modülü + Kamera Kalite Kontrol (proje aşaması) |

---

## 📂 1. Klasör: `2.1 şişeleme föyleri` (7 Laboratuvar Föyü)

| Föy No | Laboratuvar Adı | Doldurulmuş PDF Föyü | Çıktı Belgesi |
| :---: | :--- | :--- | :--- |
| **LAB 1** | **Safety Architecture** | [`LAB1_Safety_Architecture.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB1_Safety_Architecture.pdf) | **EP 03:** Safety Function Map |
| **LAB 2** | **IEC 62443 Mini Workshop** | [`LAB2_IEC62443_Mini_Workshop.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB2_IEC62443_Mini_Workshop.pdf) | **EP 05:** Zone / Conduit Diagram |
| **LAB 3** | **Threat & Risk + Risk Matrix** | [`LAB3_Threat_Risk_Matrix.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB3_Threat_Risk_Matrix.pdf) | **EP 04:** Risk Register |
| **LAB 4** | **Secure Remote Access** | [`LAB4_Secure_Remote_Access.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB4_Secure_Remote_Access.pdf) | **EP 02 + EP 06:** Secure Architecture |
| **LAB 5** | **SBOM / CVE / Patch** | [`LAB5_SBOM_CVE_Patch.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB5_SBOM_CVE_Patch.pdf) | **EP 09 · 10 · 11:** Vulnerability Decision |
| **LAB 6** | **CRA Incident Simulation** | [`LAB6_CRA_Incident_Simulation.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB6_CRA_Incident_Simulation.pdf) | **EP 13:** Incident Workflow |
| **LAB 7** | **AI Safety Challenge** | [`LAB7_AI_Safety_Challenge.pdf`](./2.1%20%C5%9Fi%C5%9Feleme%20f%C3%B6yleri/LAB7_AI_Safety_Challenge.pdf) | **EP 03 + EP 15:** AI Fail-Safe Decision |

---

## 📂 2. Klasör: `2.2 paketleme föyleri` — Kendi Makinemiz (Yılmaz Makina YILPAK DPC 500) İçin Hazırlanan 7 Laboratuvar

| Föy No | Laboratuvar Adı | Doldurulmuş PDF Föyü (Kendi Makinemiz) | Çıktı Belgesi |
| :---: | :--- | :--- | :--- |
| **LAB 1** | **Safety Architecture** | [`2_2_Foy_1_Safety_Architecture.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_1_Safety_Architecture.pdf) | **EP 03:** Safety Function Map |
| **LAB 2** | **IEC 62443 Mini Workshop** | [`2_2_Foy_2_IEC_62443_Mini_Workshop.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_2_IEC_62443_Mini_Workshop.pdf) | **EP 05:** Zone / Conduit Diagram |
| **LAB 3** | **Threat & Risk + Risk Matrix** | [`2_2_Foy_3_Threat_Risk_Matrix.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_3_Threat_Risk_Matrix.pdf) | **EP 04:** Risk Register |
| **LAB 4** | **Secure Remote Access** | [`2_2_Foy_4_Secure_Remote_Access.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_4_Secure_Remote_Access.pdf) | **EP 02 + EP 06:** Secure Architecture |
| **LAB 5** | **SBOM / CVE / Patch** | [`2_2_Foy_5_SBOM_CVE_Patch.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_5_SBOM_CVE_Patch.pdf) | **EP 09 · 10 · 11:** Vulnerability Decision |
| **LAB 6** | **CRA Incident Simulation** | [`2_2_Foy_6_CRA_Incident_Simulation.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_6_CRA_Incident_Simulation.pdf) | **EP 13:** Incident Workflow |
| **LAB 7** | **AI Safety Challenge** | [`2_2_Foy_7_AI_Safety_Challenge.pdf`](./2.2%20paketleme%20f%C3%B6yleri/2_2_Foy_7_AI_Safety_Challenge.pdf) | **EP 03 + EP 15:** AI Fail-Safe Decision |

---

## 📊 3. Stratejik Analiz: SWOT Analizi

Yılmaz Makina YILPAK DPC 500 için Safety 4.0 LAB 1–7 çalışmaları doğrultusunda hazırlanan stratejik analiz raporu:
* **Markdown Raporu:** [`SWOT Analizi — Yilmaz Makina YILPAK DPC 500.md`](./SWOT%20Analizi%20%E2%80%94%20Yilmaz%20Makina%20YILPAK%20DPC%20500.md)
* **PDF Belgesi:** [`SWOT Analizi — Yilmaz Makina YILPAK DPC 500.pdf`](./SWOT%20Analizi%20%E2%80%94%20Yilmaz%20Makina%20YILPAK%20DPC%20500.pdf)

---

## 👤 Hazırlayan & İletişim
* **Öğrenci:** Samet Yeşilot (`230541036`) — [@sametyesilot](https://github.com/sametyesilot)
* **Ders:** Yazılım Mühendisliğinde Güncel Konular
* **Proje Konusu:** Yılmaz Makina (SAMİB Üyesi) – **YILPAK DPC 500 Tam Otomatik Dikey Paketleme Makinesi** Safety 4.0 Mühendislik Paketi
