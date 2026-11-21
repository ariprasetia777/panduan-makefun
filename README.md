# bring-the-humans-02 — DRAFT panduan (siap publish begitu GitHub dibuat)

Deadline bounty: **Sabtu 2026-11-21 17:30 WIB** (kurang-lebih 34 jam dari Jumat pagi 2026-11-20).
Status: DRAFT — belum bisa disubmit. Blocker satu-satunya: user belum punya akun GitHub,
dan repo entry harus milik akun GitHub yang TERLINK ke akun make.fun @rapid-beacon-48
(display Jonhry77). Semua di bawah ini sudah disiapkan supaya begitu GitHub jadi,
tinggal copy-paste + submit.

## Yang harus mas lakukan (urutan, ~15 menit)

1. Bikin akun GitHub di github.com (gratis, pakai email).
2. Di make.fun, buka profil → tab Identity → link GitHub itu.
   Cek: /api/me harus nunjukin github_login terisi (kemarin masih null).
3. Ambil kode referral mas di make.fun: profil → tab Referrals.
   Link bentuknya https://make.fun/r/<kode> — ganti semua yqbeny8x di bawah.
4. Bikin repo PUBLIK baru di GitHub (nama saran: `panduan-makefun` — `makefun-guide`
   sudah dipakai Bawuk12), lisensi MIT, topik: makefun, bounties, ai-agents.
   Repo harus dibuat SETELAH bounty dibuka (18 Nov 10:30 UTC) — bikin hari ini aman.
   About repo: website https://make.fun + topik `makefun`.
5. Paste isi README di bawah sebagai README.md repo itu, commit + push.
6. Screenshot halaman repo → simpan sebagai screenshot.png di root repo.
7. Bilang ke adek: adek yang submit entry-nya dari kit (repo-url + commit + bundle
   transkrip sesi ini). Klaim hadiah tetap nunggu izin mas.

## Jujur soal peluang

Hadiah $1.000 top-50 (juara 1 $150) dibayar BERDASARKAN jumlah signup manusia
terverifikasi lewat link referral mas — bukan berdasarkan bagus-tidaknya panduan.
Panduan ini cuma kendaraannya. Dengan sisa ~34 jam, signup yang kekejar kemungkinan
kecil; yang dikejar di sini adalah: entry valid masuk sebelum deadline, dan link
referral mas jadi tersebar (X @ariprasetia77 + repo publik). Kalau mas mutusin skip,
nggak ada rugi — nggak ada uang keluar.

## Model yang dipakai

Repo Bawuk12/makefun-guide (dibuat 2026-11-19, 14,5 KB README + screenshot.png +
LICENSE) — dipelajari sampai habis 2026-11-19 malam. Struktur di bawah mengikuti
pola itu persis (3 badge di atas, link referral di awal + di akhir, urutan lengkap
daftar → cari bounty → ambil kit → grade-local → bundle → check → submit → klaim,
contoh jalan tiny-chess-01, FAQ 8 pertanyaan), tapi isinya ditulis ulang dengan
bahasa Indonesia dan contoh nyata entry mas sendiri (Adept Lattice).

Badge (ganti <github-mu> dengan username GitHub mas begitu ada):
- https://make.fun/badge/bring-the-humans-02.svg
- https://make.fun/badge/bring-the-humans-02/<github-mu>/panduan-makefun/rank.svg
- https://make.fun/badge/bring-the-humans-02/<github-mu>/panduan-makefun/reward.svg

---

# --- MULAI README (copy dari sini) ---

# Langkah Pertama di make.fun — Panduan Pemula

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun)
[![rank](https://make.fun/badge/bring-the-humans-02/<github-mu>/panduan-makefun/rank.svg)](https://make.fun)
[![reward](https://make.fun/badge/bring-the-humans-02/<github-mu>/panduan-makefun/reward.svg)](https://make.fun)

Kalau kamu belum pernah dengar [make.fun](https://make.fun), halaman ini buat kamu.
Dijelasin dengan bahasa yang gampang: apa itu make.fun, cara bikin akun, cara cari
bounty yang beneran bisa kamu bangun, dan cara masukin entry pertamamu. Nggak
diasumsikan kamu sudah pernah ikut kontes atau pakai coding agent sebelumnya.

> **Mau gabung make.fun?** Daftar lewat link referral saya:
> https://make.fun/r/yqbeny8x
>
> Kode referral saya: yqbeny8x.

## Apa itu make.fun

[make.fun](https://make.fun) adalah website tempat orang memakai AI coding agent
untuk membangun software dan memenangkan hadiah uang tunai. Hadiah dibayar dalam
USDC, cryptocurrency yang nilainya dipatok ke dolar, di jaringan Solana.

Ide dasarnya simpel:

1. Ada yang posting **bounty** — tugas membangun sesuatu, dengan hadiah, deadline,
   dan aturan yang jelas.
2. Kamu pilih bounty, bangun barangnya dengan AI coding agent, lalu submit hasilmu.
3. Semua entry dinilai dengan cara yang sama, di sandbox, dan yang terbaik
   mengambil tempat berbayar.
4. Kalau entry-mu menang, kamu klaim hadiahnya ke wallet Solana kamu sendiri.

Kamu nggak harus jadi programmer profesional. Coding agent yang nulis kodenya;
tugasmu adalah memilih tugasnya, mengarahkan agent, mengecek hasilnya, dan
memutuskan kapan submit.

## Yang kamu butuhkan

Sebelum entry pertama, siapkan empat hal ini. Semuanya gratis:

- **AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI,
  opencode, Cline, Aider, dan banyak lagi — semuanya bisa. Kalau kamu sudah
  pakai satu, terus pakai itu.
- **Akun GitHub.** Entry-mu tinggal di repo GitHub publik. Kalau belum punya,
  bikin akun itu gratis.
- **Wallet Solana.** Di sinilah hadiah dibayar. Phantom, Solflare, atau keypair
  yang dibuatkan tool make.fun — semuanya bisa. Kamu nggak perlu pegang dana
  apa pun untuk ikut.
- **Node.js 22.** Kit bounty dijalankan dengan tool command-line kecil, dan
  Node.js yang menjalankannya.

## Menyiapkan akunmu

### Langkah 1 — Daftar

Buka [make.fun](https://make.fun) dan pilih **Sign in** di pojok atas. Kamu bisa
masuk dengan GitHub, Google, Apple, Discord, atau wallet Solana. Masuk dengan
wallet tidak mengirim transaksi dan tidak dipungut biaya.

Kalau kamu pakai link referral saya, https://make.fun/r/yqbeny8x,
halaman daftar sudah tahu kodenya — kamu nggak perlu mengetik apa pun.

### Langkah 2 — Buat profilmu jadi milikmu

Klik avatar di kanan atas dan buka profilmu. Pilih username, tambah foto, dan
tulis bio satu baris. Nama inilah yang dilihat builder lain di sebelah entry-mu.

### Langkah 3 — Hubungkan sisanya

Di tab **Identity** profilmu, kamu bisa menghubungkan akun yang belum kamu pakai
waktu masuk: GitHub, Google, Apple, Discord, dan X. Menghubungkan GitHub paling
penting, karena entry-mu disubmit dari repo di bawah akun GitHub itu.
Menghubungkan wallet Solana juga penting, karena di situlah hadiah mendarat.
Kamu juga bisa menyembunyikan akun-akun itu dari profil publikmu kalau mau.

### Langkah 4 — Hubungkan tool agent-mu sekali saja

Setiap bounty dikirim dengan kit — folder berisi aturan, data latihan, dan tool
command-line. Pertama kali pakai kit, hubungkan ke akunmu supaya entry masuk
atas namamu:

```
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak link dan kode persetujuan. Buka link itu selagi kamu
sudah login, cek kodenya cocok, lalu setujui. Login pertama juga membuat keypair
Solana di komputermu, yang nantinya menandatangani entry dan klaimmu. Atur apa
saja yang boleh dilakukan koneksi itu di **Profile → API keys → Paired agents**.

## Mencari bounty yang bisa kamu bangun

Halaman depan [make.fun](https://make.fun) mengelompokkan bounty ke Trending,
New, dan Ending soon, dengan kategori seperti Code, Games, Trading, Forecasting,
dan Growth. Setiap kartu bounty menunjukkan hadiahnya. Klik satu dan baca
halamannya baik-baik sebelum membangun apa pun:

- **Tugasnya** — apa yang harus dibangun, satu baris lalu selengkapnya.
- **Aturannya** — apa yang harus ada di entry dan bagaimana penilaiannya.
- **Hadiahnya** — apa yang diterima setiap tempat berbayar.
- **Fasenya** — kapan entry ditutup dan kapan hasil diumumkan.

Bounty pertama yang bagus adalah yang tugasnya kamu pahami dalam sekali baca
dan aturannya cocok dengan tool yang sudah kamu punya. Lewati saja yang butuh
software yang tidak bisa kamu install atau akun yang tidak bisa kamu buat.
Selalu ada bounty lain yang segera dibuka.

## Dari memilih bounty sampai submit

### Ambil kit-nya

Dari halaman bounty, atau di terminal:

```
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalam kit adalah aturan bounty kata demi kata. Baca itu. Di situ
juga dibilang apakah kamu bisa menilai entry-mu sendiri di komputermu sebelum
submit.

### Mulai sesi baru

Buat repo GitHub publik baru, clone di sebelah folder kit, dan buka sesi **baru**
coding agent-mu di dalamnya. Ini penting: transkrip membuktikan agent-mu yang
mengerjakan, jadi sesi yang dimulai sebelum bounty dibuka tidak bisa diikutkan —
timestamp-nya tidak akan cocok. Tambahkan lisensi open-source seperti MIT —
entry wajib membawa lisensi.

### Bangun dengan agent-mu

Biarkan agent-mu yang menulis. Pemeriksaan membandingkan transkrip sesimu dengan
kode, jadi pekerjaan yang ditempel dari tempat lain nilainya lebih kecil. Kamu
boleh menulis sebagian kode dengan tangan; bobotnya sebagai pekerjaan agent-mu
saja yang berkurang. Kalau kit punya folder `starter/`, salin itu dan biarkan
agent-mu mengubahnya jadi entry-mu sendiri — itu titik awal yang sudah jalan,
bukan pemenang. Instruksi pertama yang berguna untuk agent-mu adalah membaca
panduan agent di [make.fun/skill.md](https://make.fun/skill.md), yang
mendokumentasikan seluruh loop entry.

### Nilai secara lokal kalau bisa

Banyak kit membiarkanmu menilai entry-mu dengan data latihan sebelum submit:

```
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Ini menjalankan penilaian yang sama di sandbox yang sama dengan yang dipakai
server. Perbaiki apa yang ditandainya selagi masih murah.

### Bundle dan cek

Bundle transkrip sesi agent-mu dari dalam folder kit:

```
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

Bundle itu menghapus kredensial dan detail pribadi, dan mencatat apa yang
membangun entry itu: prompt pembukamu, agent-nya, modelnya, dan setup-nya.
Lalu jalankan cek situs itu sendiri di komputermu — entry yang ditolak tetap
memakan satu dari jatah submit harianmu, jadi tangkap masalahnya di sini:

```
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

### Submit

Masuk dari form **Enter** di halaman bounty, atau dari kit:

```
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<kamu>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

Keypair itu adalah wallet yang dibuat waktu kamu login, dan di situlah hadiah
akan dibayar.

## Setelah kamu submit

Cek posisi entry-mu:

```
node cli/makefun.mjs status
```

Entry bergerak lewat **submitted**, **checked**, **scored**, dan kadang
**rejected**. Entry yang ditolak mencantumkan setiap cek yang gagal beserta
perbaikannya. Perbaiki dan submit lagi — kamu bisa terus submit ulang sampai
deadline, dalam batas harian bounty itu. Entry terakhirmu yang dihitung, kecuali
kamu memilih entry yang lebih awal.

Ketika hasil diumumkan dan entry-mu menempati tempat berbayar, klaim hadiahnya
dari profilmu, atau dari kit dengan claim id yang ditunjukkan `status`:

```
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

Hadiah dibayar dalam USDC di Solana ke wallet-mu sendiri, setelah penyaringan
sanksi otomatis. Jawab `--us-person yes` kalau kamu warga AS. Formulir pajak
hanya diminta di mana hukum AS mengharuskannya.

## Jalan pertama yang konkret — contoh nyata

Misalnya kamu mau mencoba bounty pertamamu akhir pekan ini. Inilah seluruh
alur dalam bentuk kecil:

1. **Jumat malam:** daftar di https://make.fun/r/yqbeny8x, hubungkan
   GitHub dan wallet-mu, dan jelajahi board untuk bounty Code yang kecil.
2. **Sabtu pagi:** unduh kit-nya, baca `RULES.txt`, buat repo publik baru, dan
   buka sesi agent baru di dalamnya.
3. **Sabtu siang:** bangun dengan agent-mu, jalankan `grade-local` kalau kit
   menyediakannya, dan perbaiki masalah yang jelas.
4. **Sabtu malam:** jalankan `bundle` dan `check`, perbaiki apa yang ditandai
   cek, lalu submit.
5. **Minggu:** jalankan `status`. Kalau ditolak, baca perbaikan yang tercantum,
   terapkan, dan submit lagi sebelum deadline.

Tidak ada satu pun dalam daftar itu yang butuh uang, dan setiap langkah bisa
dibatalkan — kamu bisa berhenti kapan saja dan mencoba lagi di bounty berikut.

### Contoh kerja: bounty engine catur

Supaya langkah-langkah di atas konkret, inilah bentuknya untuk satu jenis bounty
nyata di board — engine catur kecil, bounty `tiny-chess-01`. Contoh ini diambil
dari entry yang benar-benar saya submit: **"Adept Lattice"** — engine 4.035
byte (batas 4.096), Elo latihan lokal 1.464, di atas baseline rumah ±1.325,
dan lolos ke final:

```
# 1. Ambil kit (slug adalah nama bounty di URL halamannya)
curl -sSL "https://make.fun/c/tiny-chess-01/kit" | tar xz
cd tiny-chess-01-kit
cat RULES.txt          # baca aturannya dulu — selalu

# 2. Buat repo baru untuk entry, di sebelah folder kit
cd ..
gh repo create my-chess-engine --public --clone   # atau buat di github.com
cd my-chess-engine
git commit --allow-empty -m "Start"               # supaya repo punya commit pertama

# 3. Buka sesi agent BARU di folder ini dan bangun.
#    Minta agent membaca make.fun/skill.md dulu, lalu README kit.

# 4. Dari dalam folder kit, nilai dengan data latihan (kalau kit menyediakannya)
cd ../tiny-chess-01-kit
node cli/makefun.mjs grade-local --kit . --bot ../my-chess-engine --driver docker

# 5. Bundle transkrip dan jalankan cek situs
node cli/makefun.mjs bundle --repo ../my-chess-engine --out transcripts.tar.gz
node cli/makefun.mjs check --kit . --repo ../my-chess-engine --transcripts transcripts.tar.gz

# 6. Push, catat commit, lalu submit
cd ../my-chess-engine && git push
git rev-parse HEAD   # ini commit yang kamu masukkan
cd ../tiny-chess-01-kit
node cli/makefun.mjs submit --competition tiny-chess-01 \
  --repo-url https://github.com/<kamu>/my-chess-engine --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json

# 7. Pantau hasilnya
node cli/makefun.mjs status
```

Ganti `<kamu>` dengan username GitHub-mu dan `<sha>` dengan commit dari langkah
6. Kalau `check` gagal, perbaiki apa yang disebutkannya dan jalankan ulang —
itu jauh lebih murah daripada entry yang ditolak, yang tetap memakan satu jatah
submit harianmu. Kalau entry ditolak setelah submit, `status` mencantumkan cek
yang gagal dan perbaikannya; perbaiki dan submit lagi sebelum deadline.

## Referral — link-mu sendiri

Setiap akun mendapat link referral berbentuk `https://make.fun/r/<kode>` —
menambah `?ref=<kode>` ke halaman make.fun mana pun hasilnya sama. Kamu bisa
menemukannya di tab **Referrals** profilmu, bersama dengan apa yang sudah kamu
hasilkan. Kamu mendapat reward USDC ketika orang daftar lewat link-mu dan ikut
serta — misalnya dengan memasukkan bounty — ditambah bagian dari apa yang mereka
menangkan untuk sementara waktu setelah mereka bergabung. make.fun membayar
bagian itu di atas, jadi hadiah mereka sendiri tetap utuh. Hanya akun baru yang
benar-benar ikut serta yang dihitung, dan setiap reward ditinjau setidaknya
sehari sebelum bisa diklaim.

Punyaku: https://make.fun/r/yqbeny8x — kode yqbeny8x.
Kalau panduan ini membantumu memulai, memakainya adalah cara yang baik untuk
berterima kasih.

## Pertanyaan yang sering ditanyakan

**Apakah saya harus bisa coding untuk ikut?**
Tidak. Agent-mu yang menulis kodenya. Kamu memilih bounty, mengarahkan agent,
mengecek hasilnya, dan memutuskan kapan submit.

**Apakah ikut bounty butuh uang?**
Tidak, untuk bounty gratis. Beberapa bounty mengenakan fee kecil sekali jalan
untuk submit — halaman bounty selalu menunjukkannya sebelum kamu submit.
Jangan pernah membayar fee untuk bounty yang hadiahnya tidak sebanding.

**Saya tidak punya kartu kredit / akun berbayar — bisa?**
Bisa. Daftar gratis, kit gratis, submit bounty gratis tidak butuh pembayaran
apa pun. Wallet Solana untuk menerima hadiah juga gratis dibuat.

**Apa itu keypair dan apakah aman?**
Keypair adalah pasangan kunci wallet Solana yang dibuat tool make.fun waktu
kamu login pertama kali. File-nya ada di komputermu sendiri
(`~/.makefun/keypairs/`). Jangan pernah membagikan file itu ke siapa pun —
siapa pun yang memegangnya bisa mengklaim hadiahmu.

**Kenapa entry saya ditolak (rejected)?**
Biasanya karena cek otomatis menemukan masalah: repo bukan publik, lisensi
tidak ada, transkrip tidak cocok dengan kode, atau commit yang disubmit bukan
commit terakhir yang di-push. Jalankan `status`, baca daftar perbaikannya,
perbaiki, dan submit lagi sebelum deadline.

**Berapa kali saya boleh submit?**
Sampai deadline, dalam batas harian bounty itu (biasanya 10 submit per hari,
20 total). Entry terakhir yang dihitung, kecuali kamu memilih entry yang lebih
awal. Jadi submit lebih awal, lalu perbaiki dan submit ulang kalau perlu.

**Kapan hadiah dibayar?**
Setelah hasil final diumumkan dan entry-mu menempati tempat berbayar, kamu
klaim dari profilmu. Pembayaran USDC di Solana, setelah penyaringan sanksi
otomatis. Klaim biasanya harus dilakukan dalam 7 hari setelah hasil diumumkan.

**Apakah saya bisa ikut bounty yang sama dengan dua akun?**
Jangan. Satu orang satu akun. Akun ganda bisa membuat semua entry-mu
didiskualifikasi.

## Ke mana selanjutnya

- [make.fun](https://make.fun) — board bounty
- [make.fun/skill.md](https://make.fun/skill.md) — panduan agent
- Bounty yang bagus untuk pemula: cari yang tugasnya kamu pahami dalam sekali
  baca dan aturannya cocok dengan tool yang sudah kamu punya.

# --- AKHIR README ---

## Catatan untuk adek (saat submit nanti)

- Kit bring-the-humans-02: ambil via `curl -sSL "https://make.fun/c/bring-the-humans-02/kit" | tar xz`
  (belum diambil — jangan submit tanpa kit + check).
- Deliverable resmi: repo publik + README memuat kode referral + 3 badge line
  dipertahankan + screenshot halaman repo + transkrip sesi agent yang membangun
  README ini (bundle dari kit). Lisensi OSI (MIT).
- Repo harus milik akun GitHub yang terlink ke @rapid-beacon-48; /api/me 18 Nov
  masih github_login null.
- Jangan submit tanpa GitHub terlink — entry akan gagal gate.
