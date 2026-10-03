# Cyber Analog Speedometer JG:VRP

Custom HUD Speedometer Analog bergaya **Cyberpunk / Dark Neon** yang dirancang khusus untuk Jogjagamers GTA:VRP (CEF / SA-MP / RAGEMP).

## ✨ Fitur & Karakteristik Desain

1. **Dial & Gauge Speedometer Analog**:
   - Bentuk circular gauge sport racing dengan efek **Dark Glassmorphism** (`#080e18`) dan bezel bercahaya neon cyan (`#00f0ff`).
   - Garis ukur (*ticks*) dan angka kecepatan (0–200) di-generate secara matematis menggunakan SVG beresolusi tinggi (tajam di resolusi 1080p, 2K, hingga 4K).
   - Zona kecepatan tinggi (160–200) memiliki aksen *redline neon* (`#ff2a55`).
   - Jarum penunjuk analog (*needle*) menyala merah neon futuristik dengan titik pivot LED cyan, berputar halus dengan CSS transform interpolasi 60+ FPS.
   - Dynamic Speed Arc yang menyala secara progresif mengikuti jarum analog.

2. **Internal Cluster Elements**:
   - **Sen Kiri & Kanan**: Panah chevron neon hijau (`#00ff88`) yang berkedip dinamis saat aktif.
   - **Headlight Status**: Ikon lampu dengan mode redup, menyala cyan (`#00f0ff`), dan mode High Beam (`#1a8cff`).
   - **Indikator Mesin**: Ikon engine check yang menyala hijau saat mesin aktif.
   - **Indikator Seatbelt**: Peringatan merah menyala saat sabuk pengaman belum terpasang.
   - **Gear Indicator**: Badge heksagonal futuristik dengan aksen amber (`GEAR 1`, `R`, `N`).
   - **Odometer Box**: Kotak digital LCD di bagian bawah dial dengan format desimal (`0.0 MI` / `KM`).
   - **RPM Arc & Segmen Bar**: Arc RPM dinamis di dalam dial yang berubah menjadi merah menyala saat mencapai *redline* (> 85% RPM), sinkron dengan 8 blok segmen LED.

3. **Cluster Health & Fuel Bar**:
   - Terletak di sisi kiri dial gauge dalam kapsul glassmorphism gelap.
   - **Health Bar**: Bar vertikal liquid neon cyan-hijau dengan peringatan merah saat HP kritis (≤ 25%).
   - **Fuel Bar**: Bar vertikal liquid neon amber-orange dengan peringatan merah saat bensin kritis (≤ 15%).

4. **Kompatibilitas Penuh API JG:VRP**:
   File ini 100% kompatibel dan siap pakai dengan fungsi resmi dari JG:VRP:
   - `setSpeed(speed)`
   - `setSpeedMode(mode)`
   - `setRPM(rpm)`
   - `setFuel(fuel)`
   - `setHealth(health)`
   - `setGear(gear)`
   - `setEngine(state)`
   - `setHeadlights(state)`
   - `setLeftIndicator(state)`
   - `setRightIndicator(state)`
   - `setSeatbelts(state)`
   - `setOdometer(distance)`

5. **Built-in Interactive Test Controller**:
   - Jika file `index.html` dibuka langsung di browser (Chrome / Edge / Firefox), terdapat tombol `⚡ DEMO HUD` di pojok kiri atas untuk menguji slider kecepatan, RPM, status lampu, sen, bensin, dan simulasi **Auto Drive**.
   - Tombol demo dapat disembunyikan kapan saja atau ditekan `F2` untuk toggle.