# Kit PD — PEMBINA Shah Alam

Dua laman statik (web + telefon), untuk kegunaan Penggerak Dakwah. Tiada pemasangan.

| Fail | Fungsi |
|---|---|
| `index.html` | **Kit PD** — Keahlian (senarai induk MUT/MUH/Muayyid + BPMy), Minit & Tindakan, Wasilah (senarai + kalendar), Tuntutan. |
| `gagasan.html` | **Kad Gagasan** — Visi & Misi · Objektif · Gagasan · **Rujukan** (bahan PD). |

Berpaut: butang **Gagasan** pada Kit PD; **← Kit PD** pada kad gagasan.

## Keahlian
- Tab **Keahlian** = senarai induk semua ahli. Tapis: Semua / Mutabaah / Muhib / Muayyid, dan ikut PD, minat usrah, minat AJK, bilangan sesi, aktif/tidak aktif. Nama disusun ikut abjad; setiap baris boleh diklik untuk buka.
- Butiran penuh: universiti, bidang, tarikh mula/tamat pengajian, alamat cawangan & kampung, 2 tag PD, tajmik, passing ke cawangan lain (pautan borang).
- **MUT**: kehadiran direkod ikut sesi (Usrah / Program / DF + tarikh + oleh PD); bilangan sesi tertera; boleh tanda tidak aktif; minat usrah & minat AJK.
- **MUH**: Borang Pencalonan Muayyid (BPMy) penuh — 5 ciri berwajaran, skor 0–5, lulus ≥50%; remarks setiap ciri; program jadi AJK; **Export BPMy (Excel)**.
- **📊 Frekuensi usrah/program/DF ikut PD** (dalam tab Keahlian).
- **Muat senarai nama (Excel/CSV)** dari menu ⋮ — lajur `Nama` wajib; pilihan: `Universiti, Bidang, PD, PD2, Peringkat, Telefon`.

## Minit, Wasilah, Tuntutan
- **Minit**: tajuk tersuai, tarikh, kehadiran, agenda, minit + tindakan (PIC/tarikh/status). Kotak Tindakan Terbuka mengumpul semua yang belum selesai.
- **Wasilah**: nama program, bahan, perincian (tarikh, target, venue, budget), medium, PIC, status, dapatan (MUH/MUT). Papar sebagai **senarai** atau **kalendar**.
- **Tuntutan**: format ala BrioHR; jenis "Bajet Muayyasah" membuka medan agensi, akaun bank, jumlah dipohon dll.

## Data & deploy
- Disimpan dalam pelayar peranti (localStorage). **Simpan/Muat JSON** untuk backup & pindah peranti; **Export CSV/Excel** untuk Sheets.
- GitHub Pages: upload `index.html`, `gagasan.html`, `README.md` ke satu repo → Settings → Pages → main / root.

## Belum siap (menunggu bahan)
- Tab **Rujukan** pada gagasan: kad untuk Kit Kemenjadian PD, Modul & Silibus Usrah, Bahan Usrah (Kalam Dakwah), Gagasan Deck — pautan & kata laluan akan dimasukkan setelah dikongsi.
