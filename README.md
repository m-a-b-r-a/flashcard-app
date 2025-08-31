# Flashcard AI Generator

## Project Overview

Flashcard AI Generator adalah aplikasi berbasis web yang membantu pengguna membuat flashcard secara otomatis untuk keperluan belajar.  
Proyek ini lahir dari permasalahan umum: banyak pelajar atau profesional kesulitan membuat bahan belajar yang ringkas dan terstruktur.  
Dengan aplikasi ini, pengguna hanya perlu memasukkan materi (teks, artikel, atau catatan), lalu sistem akan secara otomatis menghasilkan flashcard yang siap digunakan.

Pendekatan proyek:

1. Menyediakan halaman antarmuka sederhana (single-page app) dengan alur sederhana.
2. Memanfaatkan AI untuk generate flashcard otomatis.
3. Menyimpan flashcard ke dalam deck agar dapat digunakan ulang.

---

## Technologies Used

- **Frontend**: Javascript + Tailwind CSS  
  → Dipilih karena mendukung pengembangan UI modern, cepat, dan responsif.
- **AI Integration**: GROQ (free)
  → Untuk menganalisis teks dan menghasilkan flashcard otomatis.

---

## Features

1. **AI Flashcard Generator**

   - Pengguna memasukkan teks / materi belajar.
   - AI otomatis mengekstrak poin penting menjadi pertanyaan & jawaban.

2. **Deck Management**

   - Menyimpan flashcard ke dalam deck.
   - Mengakses kembali deck yang sudah tersedia.

3. **Responsive Single Page Design**
   - Seluruh fitur tersedia dalam satu halaman (SPA).
   - Navigasi halus dan ramah pengguna.

---

## 🤖 AI Support Explanation

AI berperan penting dalam proyek ini:

- **Input → AI Processing → Output**
Dalam pengembangan proyek ini, IBM Granite digunakan sebagai **partner kolaboratif** pada berbagai tahap proses. Alurnya adalah sebagai berikut:

1. **Brainstorming Ide**  
   Menggunakan AI untuk mengeksplorasi ide awal, menganalisis kebutuhan, dan memastikan manfaatnya relevan bagi saya maupun pengguna umum.  

2. **Mendapatkan Feedback Konsep**  
   Setelah ide terbentuk, saya menjelaskannya kepada AI (IBM Granite) untuk memperoleh masukan tambahan.  

   - **Contoh Prompt (Role Prompting):**  
     > "Anda adalah seorang *Product Designer*. Analisis ide saya tentang aplikasi flashcard AI berikut, sebutkan kelebihan, kekurangan, dan potensi fitur tambahan."  

3. **Generasi Kode Awal**  
   AI digunakan untuk membuat *boilerplate code* atau draft implementasi fitur.

4. **Refinement Logic & Enhancement**  
   Memberi masukan ke AI untuk meningkatkan kualitas logic, menambah validasi, atau menyusun ulang arsitektur kode.  

   - **Contoh Prompt (Iterative Prompting):**  
     > "Refactor kode sebelumnya agar lebih clean dengan memisahkan komponen menjadi CardForm dan CardList, serta buat ketika flashcard deck name sudah ada, akan update flashcard tersebut"  

5. **Refinement UI/UX**  
   Setelah fitur berjalan, saya menggunakan AI untuk mencoba enhance UI yang telah di generate sebelumnya.  

   - **Contoh Prompt (Role Prompting - UI/UX Expert):**  
     > "Anda adalah seorang *UI/UX Designer*. Bagaimana cara memperbaiki tampilan form flashcard agar lebih menarik dan mudah digunakan? Sertakan contoh kode Tailwind."  

### CONCLUSION
Dari pengalaman menggunakan IBM Granite dalam proyek ini, terdapat beberapa point yang saya dapat:

1. **AI sebagai Partner, bukan Pengganti**  
   AI mampu menghasilkan ide, kode, dan desain dengan cepat. Namun, tetap diperlukan *judgment manusia* untuk menilai relevansi, memperbaiki kesalahan, dan memastikan hasil sesuai kebutuhan nyata.

2. **Iterative Prompting Lebih Efektif**  
   Satu kali prompt jarang menghasilkan solusi sempurna. Proses *iterasi prompt → output → refine* jauh lebih efisien dan produktif.

3. **Kualitas Prompt = Kualitas Output**  
   Memberikan konteks yang jelas (role-based, contoh format, atau constraint tertentu) menghasilkan output yang lebih sesuai dibanding sekadar zero-shot.

4. **Kombinasi Gaya Prompting**  
   Setiap tahap membutuhkan gaya prompt berbeda:  
   - *Zero-Shot* → eksplorasi ide.  
   - *Role-Based* → validasi & kritik.  
   - *Code Generation* → menghasilkan draft awal.  
   - *Few/One-Shot* → menjaga konsistensi format atau logic.  

5. **AI Mempercepat, Manusia Menyempurnakan**  
   AI mempercepat tahap awal (ideasi, boilerplate, desain kasar), sementara penyempurnaan akhir tetap membutuhkan kreativitas dan ketelitian manusia.
