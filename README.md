# 🧠 Neuro-Symbolic Engine

![Python](https://img.shields.io/badge/Python-3.13-blue.svg)
![Z3 Theorem Prover](https://img.shields.io/badge/Z3-SMT_Solver-red.svg)
![Gemini AI](https://img.shields.io/badge/Gemini-LLM-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**Neuro-Symbolic Engine**, yazılım güvenliğini otomatize etmek için **Microsoft Z3 Sembolik İspat Motoru'nun** matematiksel kesinliği ile **Büyük Dil Modellerinin (Gemini LLM)** üretken onarım yeteneklerini birleştiren hibrit ve otonom bir güvenlik ekosistemidir.

Sistem, geleneksel statik analiz araçlarının veya tek başına çalışan yapay zeka modellerinin aksine, kod açıklarını istatistiksel olarak tahmin etmez; uzaydaki tüm olasılıkları test ederek **matematiksel olarak ispatlar** ve otonom bir şekilde **onarır**.

---

## 🚀 Temel Özellikler ve Modüller

Proje, standart yazılım süreçlerinden blokzincir ekosistemine kadar geniş bir yelpazede güvenlik sağlayan 6 çekirdek modülden oluşmaktadır:

### 1. Çalışma Zamanı (Runtime) Koruması
Temel aritmetik, sınır aşımları (Index Out of Bounds) veya mantıksal sızıntılar gibi çalışma zamanında uygulamanın çökmesine yol açacak hataları, kod daha çalıştırılmadan tespit eder ve düzeltir.

### 2. Otonom CI/CD Pull Request (PR) Botu
DevOps süreçleri için geliştirilmiş otonom bir ajandır. GitHub deposunu izler, yeni gönderilen kodlarda matematiksel bir mantık hatası bulursa inşayı (build) durdurur. Hatayı LLM ile onarır ve repoya doğrudan **"Otonom Güvenlik Yaması"** adıyla yeni bir PR (Pull Request) açar.

### 3. Kendi Kendini Onaran (Self-Healing) Derleyici Katmanı
Özel programlama dilleri ve hibrit derleyiciler için tasarlanmış **Semantik Analiz** katmanıdır. Derleyici, hatalı kodu reddetmek yerine arka planda otonom olarak düzeltir ve sadece %100 matematiksel onayı alınmış kodları derler.

### 4. Asenkron Durum (State) Yönetimi Doğrulayıcısı
Özellikle modern mobil ve web uygulamalarındaki karmaşık mimari çökmeleri hedefler. Asenkron API çağrıları sırasındaki yarış durumlarını (Race Conditions) ve UI yaşam döngüsü (Lifecycle) çakışmalarını henüz kod çalışmadan ispatlar.

### 5. Akıllı Kontrat (Web3) Denetimi
Blokzincir tabanlı (Solidity/Rust) akıllı kontratları denetler. Tamsayı Taşması (Integer Underflow), Bakiye Üstü Çekim (Overdraw) veya Reentrancy gibi finansal zafiyetleri ve hack senaryolarını matematiksel ispat yöntemiyle yakalar.

### 6. Görsel İspat ve AST Haritalama (Visual Reasoning)
Sistemin analiz süreçlerini şeffaflaştıran "Açıklanabilirlik" modülüdür. Z3 motorunun hata bulurken izlediği mantıksal yolu, değişkenleri ve Soyut Sözdizimi Ağacını (AST) **Graphviz** kullanarak çizer. Hataya sebep olan düğümler haritada açıkça vurgulanır.

---

## 🛠 Mimari ve Teknoloji Yığını

Bu sistem, izole bir script olmaktan ziyade ölçeklenebilir bir **Backend-as-a-Service (BaaS)** mimarisine uygun tasarlanmıştır.

* **Sembolik Çözücü:** Z3 Theorem Prover (SMT)
* **Nöral Sentez Katmanı:** Google GenAI (Gemini API)
* **AST Ayrıştırıcı:** Python `ast` kütüphanesi
* **Görselleştirme:** Graphviz
* **DevOps Entegrasyonu:** PyGithub REST API

---

## Görseller
<img width="1264" height="703" alt="image" src="https://github.com/user-attachments/assets/c7975920-1dc3-428d-85d2-98e3271e1eb2" />
<img width="1258" height="709" alt="image" src="https://github.com/user-attachments/assets/dc8436c7-1e85-4900-a698-983d9e4cbc60" />
<img width="1255" height="699" alt="image" src="https://github.com/user-attachments/assets/cd147b10-bac0-4467-aafc-01132d8b8b04" />
<img width="1262" height="706" alt="image" src="https://github.com/user-attachments/assets/e2240c16-695e-4eeb-9f9d-191dafa21e8a" />
<img width="1260" height="706" alt="image" src="https://github.com/user-attachments/assets/408d1f15-eab3-4e99-ba14-62f1d355015f" />
<img width="1258" height="702" alt="image" src="https://github.com/user-attachments/assets/97cbadc0-3b1f-496b-aa17-a2d19acf8e9b" />
<img width="1257" height="712" alt="image" src="https://github.com/user-attachments/assets/dc01453b-e866-47f2-9945-2e37f3afd303" />
<img width="1261" height="708" alt="image" src="https://github.com/user-attachments/assets/4f325c07-a7e6-4777-bf96-2067239c361f" />
<img width="1260" height="606" alt="image" src="https://github.com/user-attachments/assets/f36f3f77-9901-4907-999e-7ba56490158c" />

## 👩‍💻 Geliştirici

**Elif Nur Ayhan**
