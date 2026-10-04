# Cyber Analog Speedometer JG:VRP

Custom HUD Speedometer Analog bergaya **Cyberpunk / Dark Neon** yang dirancang khusus untuk JGV:RP FiveM

## ✨ Karakteristik Desain & Tata Letak Terintegrasi (Compact Single-Dial)

1. **Integrated All-in-One Circular Gauge**:
   - Desain piringan tunggal kompak tanpa panel terpisah di sisi luar.
   - Efek **Dark Glassmorphism** (`#080e18`) dengan ring luar neon cyan (`#00f0ff`) dan bezel grid futuristik.
   - Jarum penunjuk (*needle*) analog neon crimson-red berputar presisi pada poros tengah.

2. **Integrasi Bar HP (Health) & GAS (Fuel) di Dalam Piringan**:
   - Bar **HP** ditempatkan di sisi kiri dalam piringan dial dengan track cyber vertikal dan persentase numerik cyan (`#00ffcc`).
   - Bar **GAS** ditempatkan di sisi kanan dalam piringan dial dengan track cyber vertikal dan persentase numerik amber (`#ff9d00`).
   - Kedua bar berubah menjadi peringatan merah menyala saat kondisi kritis (HP ≤ 25%, Bensin ≤ 15%).

3. **Teks Kecepatan & Unit (MPH / KMH / KNOTS)**:
   - Terletak di area tengah atas dial, tersusun vertikal secara rapi.
   - Bebas dari tumpukan jarum dan tutup poros (*needle cap*), memberikan keterbacaan instan yang tajam.

4. **Cluster Status Bawah (Near Gear Box)**:
   - Bar status horizontal yang memuat 5 indikator bersebelahan:
     `[ Sen Kiri ◀ ]  [ 💡 Headlights ]  [ ⚙️ Engine ]  [ 🛡️ Seatbelt ]  [ Sen Kanan ▶ ]`
   - Berdampingan langsung dengan badge heksagonal **GEAR** (`GEAR 1`, `R`, `N`), **Segmen Bar RPM**, dan **Digital Odometer Box** (`0.0 MI` / `KM`).

## ⚙️ Kompatibilitas API & Fungsi Global JG:VRP

File `index.html` ini mengimplementasikan fungsi standar JG:VRP:
- `setSpeed(speed)` — Mengonversi kecepatan ($m/s$), memutar jarum analog (-135° s/d +135°), dan mengisi dynamic speed arc.
- `setSpeedMode(mode)` — Mode 0: KMH, 1: MPH, 2: Knots.
- `setRPM(rpm)` — Menggerakkan busur RPM dial & 8 segmen bar LED.
- `setFuel(fuel)` — Mengatur persentase bensin mini bar kanan (`#fuel-bar`).
- `setHealth(health)` — Mengatur persentase kondisi kendaraan mini bar kiri (`#health-bar`).
- `setGear(gear)` — Mengatur posisi gigi (`R`, `N`, `GEAR 1`, dll.).
- `setEngine(state)` — Menyalakan/mematikan lampu indikator mesin.
- `setHeadlights(state)` — 0: Off, 1: On (Cyan), 2: High Beam (Biru).
- `setLeftIndicator(state)` — Indikator sen kiri berkedip hijau.
- `setRightIndicator(state)` — Indikator sen kanan berkedip hijau.
- `setSeatbelts(state)` — Peringatan sabuk pengaman merah menyala jika belum dipasang.
- `setOdometer(distance)` — Memperbarui angka jarak tempuh digital.

## 🧪 Browser Testing & Demo Controller

- Buka langsung file `index.html` di browser apa pun untuk menguji tampilan.
- Klik tombol **`⚡ DEMO HUD`** di pojok kiri atas atau tekan tombol keyboard **`F2`** untuk membuka panel pengujian (slider speed, rpm, hp, gas, dan tombol simulasi **Auto Drive**).
