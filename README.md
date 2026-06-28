# ⚡ Rekayasa Panel Motor Control Center (MCC) Star-Delta
**Penerapan Pengasutan Star-Delta untuk Sistem Pemompaan Tekanan Tinggi Industri**

Proyek ini berisi draf rekayasa kelistrikan lengkap (*blueprint* daya dan kontrol) serta file simulasi untuk panel *Motor Control Center* (MCC) berstandar PUIL 2011 dan IEC. Sistem ini dirancang khusus untuk memitigasi *inrush current* pada motor induksi penggerak pompa *slurry* atau sentrifugal di fasilitas industri berat.

## 📂 Isi Repositori
* **📄 Engineering Report:** Laporan teknis komprehensif (Format PDF).
* **📐 QElectroTech Schematics:** File sumber desain sirkuit daya (380VAC) dan sirkuit kontrol logika sekuensial (24VDC).
* **🖥️ SimulIDE Simulation:** File laboratorium virtual untuk simulasi waktu-nyata (*real-time*).

## 🛠️ Fitur Teknis & Parameter Keamanan
1. **Transisi Sekuensial:** Menggunakan *Time Delay Relay* (TDR) dengan kalibrasi waktu absolut 7 detik untuk perpindahan Star ke Delta.
2. **Proteksi Interlok Berlapis:** Implementasi *Hardwired Electrical Cross-Interlock* pada terminal kontak bantu NC 21-22 untuk memblokir risiko hubung singkat fasa-ke-fasa.
3. **Fail-Safe Mode:** Simulasi *trip* beban lebih (Overload) yang divalidasi melalui respons instan *Thermal Overload Relay* (TOR) terminal 95-96 dan 97-98.
4. **Reverse Engineering Analysis:** Pengujian sabotase *bypass interlock* untuk memetakan rute kegagalan sistem operasional.

## 🚀 Cara Menjalankan Simulasi
1. Unduh dan instal [SimulIDE](https://www.simulide.com/).
2. Unduh file `.simu` dari repositori ini.
3. Buka file tersebut di SimulIDE dan tekan tombol **Power (Run)** warna merah di atas layar.
4. Tekan sakelar *Start* (NO) untuk memulai sekuens asut.

---
*Proyek ini merupakan portofolio simulasi independen yang dirancang untuk mendemonstrasikan kapabilitas rekayasa otomasi industri dan pemahaman terhadap regulasi proteksi kelistrikan motor 3-fase.*
