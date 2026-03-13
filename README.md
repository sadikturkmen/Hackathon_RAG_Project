# Smart Document Analyst (PDF & Reporting)

This project is an AI-powered application that analyzes uploaded PDF files, answers user questions, and returns results in a structured report format (`Question`, `Answer`, `Agent Comment`, `Action Suggestions`).

## Installation

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Configure your `.env` file (or provide values from the app UI):
   - `GOOGLE_API_KEY`: Google Gemini API key
   - `SENDER_EMAIL` and `SENDER_PASSWORD`: credentials for email reporting (optional)

## Usage

Start the app with:

```bash
streamlit run app.py
```

## Features
- **PDF Processing**: Reads and chunks PDF content, then stores vectors in Chroma.
- **RAG-based Answers**: Uses Gemini + retrieval to answer questions based on document context.
- **Structured Output**: Returns response as `Question / Answer / Agent Comment / Action Suggestions`.
- **Email Reporting**: Can send generated analysis via email.

---

# Akıllı Doküman Analisti (PDF ve Raporlama)

Bu proje, yüklenen PDF dosyalarını analiz eden, kullanıcı sorularını yanıtlayan ve sonuçları yapılandırılmış bir rapor formatında (`Soru`, `Cevap`, `Agent Yorumu`, `Öneri Aksiyonları`) sunan yapay zeka destekli bir uygulamadır.

## Kurulum

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install -r requirements.txt
   ```

2. `.env` dosyanızı yapılandırın (veya değerleri uygulama arayüzünden girin):
   - `GOOGLE_API_KEY`: Google Gemini API anahtarı
   - `SENDER_EMAIL` ve `SENDER_PASSWORD`: e-posta raporlama için kimlik bilgileri (opsiyonel)

## Kullanım

Uygulamayı başlatmak için:

```bash
streamlit run app.py
```

## Özellikler
- **PDF İşleme**: PDF içeriğini okur, parçalara böler ve Chroma içinde vektör olarak saklar.
- **RAG Tabanlı Yanıt**: Doküman bağlamına göre Gemini + retrieval ile soru yanıtlar.
- **Yapılandırılmış Çıktı**: Yanıtı `Soru / Cevap / Agent Yorumu / Öneri Aksiyonları` formatında üretir.
- **E-posta Raporlama**: Üretilen analizi e-posta ile gönderebilir.