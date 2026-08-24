# Kit PD · PEMBINA Shah Alam

Suite ringkas untuk pengurusan gerak kerja tarbiah PSPB 2026 (Mutabaah → Muhib → Muayyid).

## Fail dalam repo ini

| Fail | Guna |
|---|---|
| `index.html` | **Kit PD** — aplikasi utama PD: keahlian, log usrah & kehadiran, minit & tindakan, wasilah, tuntutan, rujukan. |
| `papan-psm.html` | **KPI PSM** — papan pemuka (baca sahaja) untuk pantau KPI, IPT, PD, kalendar usrah & notifikasi perubahan. |
| `gagasan.html` | **Kad Gagasan** — rujukan produk gagasan. |
| `Code.gs` | **Backend Google Apps Script** — simpan/gabung data, muat naik lampiran, backup harian. |

## Model data & keselamatan

- Semua data disimpan dalam **satu Google Sheet**, diakses melalui **satu Apps Script** (`Code.gs`).
- Akses dilindungi oleh **satu kod pasukan** (`SECRET` dalam `Code.gs`) — kod ini **tidak** disimpan dalam HTML.
- URL `/exec` dibakar dalam `index.html` & `papan-psm.html` (cari `APPS_SCRIPT_URL`).
- **Privasi:** aplikasi menyimpan **tarikh lahir** (bukan nombor IC penuh) untuk hari lahir. Rekod lama yang ada IC akan ditukar ke tarikh lahir & IC dipadam secara automatik apabila dibuka.

## Cara deploy

1. **Backend:** Extensions → Apps Script, tampal `Code.gs`, simpan. Deploy → New/Manage deployment → Web app (Execute as Me, Anyone).
2. Jalankan `authorizeDrive` sekali (benarkan Google Drive) untuk lampiran.
3. Jalankan `installBackupTrigger` sekali untuk backup harian automatik (2 pagi) ke folder Drive **KitPD Backups** (30 salinan terkini disimpan).
4. **Frontend:** pastikan `APPS_SCRIPT_URL` dalam `index.html` & `papan-psm.html` = URL `/exec` anda, kemudian upload ke repo GitHub Pages.

## Backup & pemulihan

- Backup automatik harian → folder Drive **KitPD Backups** (`kitpd-backup-YYYY-MM-DD-...json`).
- `backupDaily()` boleh dijalankan manual bila-bila masa untuk snapshot segera.
- Untuk pulih: buka fail backup, ambil JSON, dan tampal semula ke Sheet (hubungi admin/dev).

## Cadangan penambahbaikan akan datang

- Tukar kod pasukan → **Google Sign-in + senarai emel** (identiti sebenar per orang).
- Bila ahli bertambah banyak: simpan **satu baris per ahli** (bukan satu blob JSON).
- Ujian aksesibiliti (fokus keyboard, aria-label) untuk pengguna telefon.

---
_Dibina secara berperingkat bersama pasukan PSM. Simpan setiap perubahan sebagai commit berasingan untuk sejarah & rollback._
