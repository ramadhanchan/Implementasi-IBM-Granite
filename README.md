# Implementasi-IBM-Granite
Dibuat oleh RAMADHAN
# Title
Classifying & Summarizing McDonald’s Store Review Using IBM Granite
# Raw Dataset Link
menggunakan dataset yang disediakan oleh kaggle 
berikut linknya https://www.kaggle.com/datasets/nelgiriyewithana/mcdonalds-store-reviews
# Project Overview
Proyek ini bertujuan untuk menganalisis ulasan pelanggan McDonald’s menggunakan AI model IBM Granite 3.3 8B Instruct.
Analisis difokuskan pada sentimen pelanggan (positif, netral, negatif) serta aspek utama ulasan seperti kualitas makanan,pelayanan, kecepatan, kebersihan, harga dan suasanan.
Pendekatan ini memanfaatkan Large Language Model (LLM) untuk mendapatkan insight lebih dalam dari data teks yang tidak terstruktur
# Analysis Process
1. Data Collection:
Mengambil dataset berisi nama toko, ulasan pelanggan, dan rating.

2. Data Cleaning:

- Menghapus nilai kosong pada kolom review.

- Mengubah semua teks menjadi huruf kecil.

-  Menghapus URL, tanda baca, angka, dan karakter non-alfabet.

Hasil akhir disimpan dalam kolom cleaned_review.

3. Sampling
 Mengambil 50 data review pertama untuk efisiensi pemrosesan. tadinya untuk training pada model ibmnya supaya gratis ternyata dari ibm granitenya cuma sediain 5 doang untuk klasifikasi.

4. AI Batch Processing:
  Mengirim setiap cleaned review ke model IBM Granite 3.3 8B Instruct untuk analisis:

- Klasifikasi sentimen (positif, netral, negatif).

- Identifikasi aspek (kualitas makanan,pelayanan, kecepatan, kebersihan, harga dan suasanan).

- Ringkasan otomatis tiap ulasan.

5. Output:
Hasil disimpan dalam dua file:

- granite_batch_results.csv → hasil klasifikasi aspek & sentimen.
  
- granite_summary_results.csv → hasil ringkasan AI per ulasan.
# Insight dan finding:
Hasil dari IBM Granite untuk klasifikasi terhadap data McDonald’s Store Review diantara lain:


- Mayoritas review (≈ 67%) bersentimen negatif, didominasi keluhan pada aspek service dan speed.

- Sentimen positif muncul hanya pada sebagian kecil review (20%) — umumnya terkait makanan.

- Sentimen netral (13%) menunjukkan review yang deskriptif tanpa emosi kuat.
  
# Visualisasi
sudah saya sisipkan 
# AI Support Explanation
Analisis ini memanfaatkan IBM Granite 3.3 8B Instruct melalui Replicate API.
Model AI digunakan untuk:

- Melakukan sentiment classification.

- Mengidentifikasi aspek ulasan (service, food, speed, cleanliness).

- Menghasilkan ringkasan singkat setiap review.

- Menyediakan insight yang konsisten tanpa bias manusia.

Dengan dukungan AI, proses analisis ratusan ulasan dapat dilakukan secara cepat, terukur, dan efisien.
