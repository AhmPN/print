
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>vutaa print — Serba 1K | Cepat & Murah bagi Pelajar</title>
    <meta name="description" content="Jasa print cepat dan murah untuk pelajar SD, SMP, SMA di Desa Pandu Senjaya, SP 4 Pangkalan Lada. Harga Serba 1K & Gratis Delivery minimal 15 lembar.">
    
    <!-- Google Fonts: Plus Jakarta Sans & Poppins -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=Poppins:wght@700;800;900&display=swap" rel="stylesheet">
    
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- QRCode.js -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                        display: ['"Poppins"', 'sans-serif'],
                    },
                    colors: {
                        navy: {
                            950: '#070D1F',
                            900: '#0B132B',
                            800: '#1C2541',
                            700: '#273459',
                        },
                        gold: {
                            400: '#FBBF24',
                            500: '#F59E0B',
                        },
                        brandOrange: {
                            500: '#F97316',
                            600: '#EA580C',
                        }
                    }
                }
            }
        }
    </script>

    <style>
        body {
            background-color: #0B132B;
            background-image: 
                radial-gradient(circle at 10% 10%, rgba(251, 191, 36, 0.12) 0%, transparent 40%),
                radial-gradient(circle at 90% 90%, rgba(249, 115, 22, 0.12) 0%, transparent 45%);
        }
        .card-surface {
            background: rgba(28, 37, 65, 0.85);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        .text-gradient-gold {
            background: linear-gradient(135deg, #FDE047 0%, #FBBF24 45%, #F97316 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        /* Hilangkan panah default input number */
        input[type=number]::-webkit-inner-spin-button, 
        input[type=number]::-webkit-outer-spin-button { 
            -webkit-appearance: none; 
            margin: 0; 
        }
        input[type=number] {
            -moz-appearance: textfield;
        }
        #qrcode img, #qrcode canvas {
            margin: 0 auto;
            display: block;
        }
    </style>
</head>
<body class="text-slate-100 font-sans antialiased min-h-screen flex flex-col justify-between selection:bg-gold-400 selection:text-navy-950">

    <!-- Toast Notification -->
    <div id="toast" class="fixed bottom-4 right-4 z-50 transform translate-y-20 opacity-0 transition-all duration-300 pointer-events-none">
        <div id="toast-box" class="bg-emerald-600 text-white px-4 py-2.5 rounded-xl shadow-2xl flex items-center gap-2.5 border border-emerald-400/30 text-xs font-bold">
            <i id="toast-icon" class="fa-solid fa-circle-check text-base"></i>
            <span id="toast-message">Berhasil disalin!</span>
        </div>
    </div>

    <!-- HEADER / NAVBAR RINGKAS -->
    <header class="sticky top-0 z-40 bg-navy-950/90 backdrop-blur-md border-b border-white/10">
        <div class="max-w-6xl mx-auto px-3 sm:px-6 h-14 sm:h-16 flex items-center justify-between gap-2">
            <!-- Brand + Badge Serba 1K -->
            <div class="flex items-center gap-2 sm:gap-3">
                <a href="#" class="flex items-center gap-2 group">
                    <div class="w-8 h-8 sm:w-9 sm:h-9 rounded-xl bg-gradient-to-br from-gold-400 to-brandOrange-600 flex items-center justify-center text-navy-950 shadow-md">
                        <i class="fa-solid fa-print text-sm sm:text-base"></i>
                    </div>
                    <span class="font-display text-lg sm:text-2xl font-extrabold tracking-tight text-white">
                        vutaa <span class="text-gold-400">print</span>
                    </span>
                </a>
                <span class="px-2.5 py-0.5 rounded-full bg-gold-400/15 border border-gold-400/40 text-gold-400 font-display font-extrabold text-[11px] sm:text-xs tracking-wide">
                    SERBA 1K
                </span>
            </div>

            <!-- Tag Jenjang & Tombol Cepat Chat WA -->
            <div class="flex items-center gap-2 sm:gap-3">
                <span class="hidden md:inline-flex items-center gap-1.5 px-3 py-1 rounded-full bg-white/5 border border-white/10 text-xs font-bold text-slate-300">
                    <i class="fa-solid fa-graduation-cap text-gold-400"></i>
                    <span>SD • SMP • SMA</span>
                </span>
                <a href="https://wa.me/6285824522033?text=Halo%20vutaa%20print,%20saya%20mau%20order%20print%20dokumen." target="_blank" rel="noopener noreferrer"
                   class="inline-flex items-center gap-1.5 px-3.5 py-2 rounded-xl bg-gradient-to-r from-emerald-500 to-emerald-600 hover:from-emerald-400 hover:to-emerald-500 text-white text-xs sm:text-sm font-bold shadow-lg shadow-emerald-600/20 transition-all active:scale-95">
                    <i class="fa-brands fa-whatsapp text-base"></i>
                    <span>Chat WA</span>
                </a>
            </div>
        </div>
    </header>

    <!-- MAIN COMPACT GRID CONTENT -->
    <main class="flex-1 max-w-6xl w-full mx-auto px-3 sm:px-6 py-4 sm:py-6 flex items-center">
        <div class="w-full grid grid-cols-1 lg:grid-cols-12 gap-4 sm:gap-5 items-stretch">
            
            <!-- KOLOM KIRI: INFO LAYANAN, DELIVERY & LOKASI/QR (7 Kolom di Desktop) -->
            <div class="lg:col-span-7 flex flex-col justify-between gap-3.5 sm:gap-4">
                
                <!-- 1. Kartu Promo & Harga 'SERBA 1K' -->
                <section class="card-surface rounded-2xl p-4 sm:p-5 relative overflow-hidden">
                    <div class="flex flex-wrap items-center justify-between gap-2 mb-3.5">
                        <div>
                            <div class="flex items-center gap-2">
                                <span class="text-[11px] font-extrabold uppercase tracking-wider text-gold-400">
                                    <i class="fa-solid fa-bolt mr-1"></i>Cepat & Murah bagi Pelajar
                                </span>
                                <span class="md:hidden px-2 py-0.5 rounded-full bg-white/10 text-[10px] font-bold text-slate-200">
                                    SD • SMP • SMA
                                </span>
                            </div>
                            <h1 class="font-display text-xl sm:text-2xl font-extrabold text-white leading-snug mt-0.5">
                                Solusi Tugas Sekolahmu — <span class="text-gradient-gold">SERBA 1K</span>
                            </h1>
                        </div>
                        <div class="px-3 py-1 rounded-xl bg-gold-400 text-navy-950 font-display font-extrabold text-xs sm:text-sm shadow-sm">
                            Rp 1.000 / Lbr
                        </div>
                    </div>

                    <!-- 3 Item Harga Sejajar Kompak -->
                    <div class="grid grid-cols-3 gap-2 sm:gap-3">
                        <!-- Hitam Putih -->
                        <div class="bg-navy-900/90 border border-white/10 rounded-xl p-2.5 sm:p-3 text-center hover:border-gold-400/40 transition-colors">
                            <div class="w-8 h-8 sm:w-9 sm:h-9 mx-auto mb-1.5 rounded-lg bg-slate-700/60 text-slate-200 flex items-center justify-center text-sm sm:text-base">
                                <i class="fa-solid fa-file-lines"></i>
                            </div>
                            <div class="text-xs sm:text-sm font-bold text-white leading-tight">Dokumen Hitam Putih</div>
                            <div class="mt-1 inline-block px-2 py-0.5 rounded-md bg-gold-400/15 text-gold-400 font-display font-extrabold text-xs">
                                1K
                            </div>
                        </div>

                        <!-- Berwarna -->
                        <div class="bg-navy-900/90 border border-white/10 rounded-xl p-2.5 sm:p-3 text-center hover:border-gold-400/40 transition-colors">
                            <div class="w-8 h-8 sm:w-9 sm:h-9 mx-auto mb-1.5 rounded-lg bg-sky-500/20 text-sky-400 flex items-center justify-center text-sm sm:text-base">
                                <i class="fa-solid fa-chart-pie"></i>
                            </div>
                            <div class="text-xs sm:text-sm font-bold text-white leading-tight">Berwarna</div>
                            <div class="mt-1 inline-block px-2 py-0.5 rounded-md bg-gold-400/15 text-gold-400 font-display font-extrabold text-xs">
                                1K
                            </div>
                        </div>

                        <!-- Full Warna -->
                        <div class="bg-navy-900/90 border border-gold-400/30 rounded-xl p-2.5 sm:p-3 text-center hover:border-gold-400 transition-colors">
                            <div class="w-8 h-8 sm:w-9 sm:h-9 mx-auto mb-1.5 rounded-lg bg-brandOrange-500/20 text-brandOrange-400 flex items-center justify-center text-sm sm:text-base">
                                <i class="fa-solid fa-image"></i>
                            </div>
                            <div class="text-xs sm:text-sm font-bold text-white leading-tight">Full Warna</div>
                            <div class="mt-1 inline-block px-2 py-0.5 rounded-md bg-brandOrange-500/20 text-brandOrange-400 font-display font-extrabold text-xs">
                                1K
                            </div>
                        </div>
                    </div>
                </section>

                <!-- 2. Kartu Info Gratis Delivery -->
                <section class="rounded-2xl bg-gradient-to-r from-gold-400 via-gold-500 to-brandOrange-600 p-3.5 sm:p-4 text-navy-950 shadow-lg shadow-brandOrange-600/15 flex items-center gap-3.5">
                    <div class="w-11 h-11 sm:w-12 sm:h-12 rounded-xl bg-navy-950 text-gold-400 flex items-center justify-center text-xl sm:text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-motorcycle"></i>
                    </div>
                    <div class="min-w-0 flex-1">
                        <div class="flex flex-wrap items-center gap-1.5">
                            <span class="px-2 py-0.5 rounded-md bg-navy-950 text-gold-400 font-display font-extrabold text-[11px] sm:text-xs uppercase tracking-wide">
                                Gratis Delivery (Min. 15 Lembar)
                            </span>
                        </div>
                        <p class="font-bold text-xs sm:text-sm text-navy-950 mt-1 leading-snug">
                            Khusus Area SP 4 Pangkalan Lada <span class="mx-1">•</span> <span class="whitespace-nowrap"><i class="fa-regular fa-clock mr-1"></i>Jam 16.30 - 20.00</span>
                        </p>
                    </div>
                </section>

                <!-- 3. Kartu Lokasi & Scan QR WhatsApp -->
                <section class="card-surface rounded-2xl p-4 sm:p-5 flex-1 flex items-center">
                    <div class="w-full flex flex-col sm:flex-row items-center justify-between gap-4">
                        <!-- Info Alamat & Nomor HP -->
                        <div class="w-full sm:w-auto flex-1 space-y-3">
                            <div class="flex items-start gap-3">
                                <div class="w-9 h-9 rounded-xl bg-gold-400/15 border border-gold-400/30 text-gold-400 flex items-center justify-center text-sm shrink-0 mt-0.5">
                                    <i class="fa-solid fa-location-dot"></i>
                                </div>
                                <div>
                                    <div class="text-[11px] font-bold uppercase tracking-wider text-slate-400">Alamat Toko</div>
                                    <div class="text-sm sm:text-base font-extrabold text-white leading-snug">
                                        Desa Pandu Senjaya RT 12 RW 3
                                    </div>
                                    <div class="text-xs text-slate-400">SP 4 Pangkalan Lada</div>
                                </div>
                            </div>

                            <div class="flex items-start gap-3 pt-2.5 border-t border-white/10">
                                <div class="w-9 h-9 rounded-xl bg-emerald-500/15 border border-emerald-400/30 text-emerald-400 flex items-center justify-center text-base shrink-0 mt-0.5">
                                    <i class="fa-brands fa-whatsapp"></i>
                                </div>
                                <div class="flex-1">
                                    <div class="text-[11px] font-bold uppercase tracking-wider text-slate-400">No. HP / WhatsApp</div>
                                    <div class="flex flex-wrap items-center gap-2 mt-0.5">
                                        <span class="text-sm sm:text-base font-extrabold text-white tracking-wide">0858-2452-2033</span>
                                        <button type="button" onclick="copyPhone()"
                                                class="px-2.5 py-1 rounded-lg bg-white/10 hover:bg-white/20 text-slate-200 text-[11px] font-bold inline-flex items-center gap-1 transition-colors active:scale-95">
                                            <i class="fa-regular fa-copy"></i>
                                            <span>Salin</span>
                                        </button>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- QR Code WhatsApp Kompak -->
                        <div class="w-full sm:w-auto flex sm:flex-col items-center justify-center gap-3 sm:gap-1.5 bg-navy-900/90 border border-gold-400/30 rounded-xl p-3 shrink-0">
                            <div class="bg-white p-2 rounded-lg relative shadow-inner">
                                <div id="qrcode"></div>
                                <!-- Ikon WA kecil di tengah QR -->
                                <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
                                    <div class="w-7 h-7 rounded-full bg-white p-0.5 shadow flex items-center justify-center">
                                        <div class="w-full h-full rounded-full bg-emerald-500 text-white flex items-center justify-center text-xs">
                                            <i class="fa-brands fa-whatsapp"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="text-left sm:text-center">
                                <div class="text-[11px] font-extrabold text-gold-400 uppercase tracking-wider">Scan QR WA</div>
                                <div class="text-[10px] text-slate-400 leading-tight max-w-[130px]">Arahkan kamera HP untuk langsung chat</div>
                            </div>
                        </div>
                    </div>
                </section>

            </div>

            <!-- KOLOM KANAN: KALKULATOR ORDER CEPAT KE WA (5 Kolom di Desktop) -->
            <div class="lg:col-span-5">
                <section class="card-surface rounded-2xl p-4 sm:p-5 h-full flex flex-col justify-between border-gold-400/30 shadow-2xl">
                    <div>
                        <!-- Header Kalkulator -->
                        <div class="flex items-center justify-between pb-3 mb-3.5 border-b border-white/10">
                            <div class="flex items-center gap-2">
                                <div class="w-8 h-8 rounded-lg bg-gold-400/20 text-gold-400 flex items-center justify-center text-sm">
                                    <i class="fa-solid fa-calculator"></i>
                                </div>
                                <div>
                                    <h2 class="font-display text-base sm:text-lg font-extrabold text-white leading-none">
                                        Kalkulator Order Cepat
                                    </h2>
                                    <p class="text-[11px] text-slate-400 mt-0.5">Hitung biaya & kirim pesanan ke WA</p>
                                </div>
                            </div>
                            <button type="button" onclick="resetCalculator()" class="text-[11px] font-semibold text-slate-400 hover:text-gold-400 transition-colors">
                                Reset
                            </button>
                        </div>

                        <form id="quickOrderForm" class="space-y-3">
                            <!-- Input Jumlah Lembar Kompak (Baris Horizontal Hemat Ruang) -->
                            <div class="space-y-2">
                                <!-- Row 1: Hitam Putih -->
                                <div class="flex items-center justify-between bg-navy-900/90 border border-white/10 rounded-xl px-3 py-2">
                                    <div>
                                        <div class="text-xs sm:text-sm font-bold text-white">Hitam Putih</div>
                                        <div class="text-[11px] text-gold-400 font-semibold">Rp 1.000 / lembar</div>
                                    </div>
                                    <div class="flex items-center gap-1.5">
                                        <button type="button" onclick="updateQty('qtyBw', -1)" class="w-8 h-8 rounded-lg bg-white/10 hover:bg-white/20 text-white font-bold text-sm flex items-center justify-center active:scale-95">-</button>
                                        <input type="number" id="qtyBw" min="0" value="0" oninput="recalculate()" aria-label="Jumlah lembar hitam putih"
                                               class="w-12 h-8 text-center rounded-lg bg-navy-950 border border-white/15 text-white font-bold text-sm focus:outline-none focus:border-gold-400">
                                        <button type="button" onclick="updateQty('qtyBw', 1)" class="w-8 h-8 rounded-lg bg-gold-400/20 hover:bg-gold-400/30 text-gold-400 font-bold text-sm flex items-center justify-center active:scale-95">+</button>
                                    </div>
                                </div>

                                <!-- Row 2: Berwarna -->
                                <div class="flex items-center justify-between bg-navy-900/90 border border-white/10 rounded-xl px-3 py-2">
                                    <div>
                                        <div class="text-xs sm:text-sm font-bold text-white">Berwarna</div>
                                        <div class="text-[11px] text-gold-400 font-semibold">Rp 1.000 / lembar</div>
                                    </div>
                                    <div class="flex items-center gap-1.5">
                                        <button type="button" onclick="updateQty('qtyColor', -1)" class="w-8 h-8 rounded-lg bg-white/10 hover:bg-white/20 text-white font-bold text-sm flex items-center justify-center active:scale-95">-</button>
                                        <input type="number" id="qtyColor" min="0" value="0" oninput="recalculate()" aria-label="Jumlah lembar berwarna"
                                               class="w-12 h-8 text-center rounded-lg bg-navy-950 border border-white/15 text-white font-bold text-sm focus:outline-none focus:border-gold-400">
                                        <button type="button" onclick="updateQty('qtyColor', 1)" class="w-8 h-8 rounded-lg bg-gold-400/20 hover:bg-gold-400/30 text-gold-400 font-bold text-sm flex items-center justify-center active:scale-95">+</button>
                                    </div>
                                </div>

                                <!-- Row 3: Full Warna -->
                                <div class="flex items-center justify-between bg-navy-900/90 border border-white/10 rounded-xl px-3 py-2">
                                    <div>
                                        <div class="text-xs sm:text-sm font-bold text-white">Full Warna</div>
                                        <div class="text-[11px] text-brandOrange-400 font-semibold">Rp 1.000 / lembar</div>
                                    </div>
                                    <div class="flex items-center gap-1.5">
                                        <button type="button" onclick="updateQty('qtyFull', -1)" class="w-8 h-8 rounded-lg bg-white/10 hover:bg-white/20 text-white font-bold text-sm flex items-center justify-center active:scale-95">-</button>
                                        <input type="number" id="qtyFull" min="0" value="0" oninput="recalculate()" aria-label="Jumlah lembar full warna"
                                               class="w-12 h-8 text-center rounded-lg bg-navy-950 border border-white/15 text-white font-bold text-sm focus:outline-none focus:border-gold-400">
                                        <button type="button" onclick="updateQty('qtyFull', 1)" class="w-8 h-8 rounded-lg bg-gold-400/20 hover:bg-gold-400/30 text-gold-400 font-bold text-sm flex items-center justify-center active:scale-95">+</button>
                                    </div>
                                </div>
                            </div>

                            <!-- Pilihan Metode Pengambilan / Delivery -->
                            <div>
                                <div class="grid grid-cols-2 gap-2">
                                    <label class="cursor-pointer">
                                        <input type="radio" name="method" value="Ambil di Tempat" checked onchange="handleMethodChange()" class="peer sr-only">
                                        <div class="p-2.5 rounded-xl bg-navy-900 border border-white/15 peer-checked:border-gold-400 peer-checked:bg-gold-400/15 transition-all text-center">
                                            <div class="text-xs font-extrabold text-white"><i class="fa-solid fa-store text-gold-400 mr-1"></i>Ambil di Tempat</div>
                                        </div>
                                    </label>
                                    <label class="cursor-pointer">
                                        <input type="radio" name="method" value="Gratis Delivery" onchange="handleMethodChange()" class="peer sr-only">
                                        <div class="p-2.5 rounded-xl bg-navy-900 border border-white/15 peer-checked:border-brandOrange-500 peer-checked:bg-brandOrange-500/15 transition-all text-center">
                                            <div class="text-xs font-extrabold text-white"><i class="fa-solid fa-motorcycle text-brandOrange-400 mr-1"></i>Gratis Delivery</div>
                                        </div>
                                    </label>
                                </div>

                                <!-- Box Validasi & Alamat Antar (Hanya tampil jika Gratis Delivery dipilih) -->
                                <div id="deliverySection" class="hidden mt-2.5 space-y-2 p-2.5 rounded-xl bg-navy-900/95 border border-brandOrange-500/30">
                                    <div id="deliveryAlert" class="text-[11px] font-semibold px-2.5 py-1.5 rounded-lg bg-amber-500/20 text-amber-300 border border-amber-400/30 leading-snug">
                                        Minimal 15 lembar khusus area SP 4 Pangkalan Lada (Jam 16.30 - 20.00).
                                    </div>
                                    <input type="text" id="deliveryAddress" placeholder="Tulis alamat / patokan antar (Area SP 4)..."
                                           class="w-full px-3 py-2 rounded-lg bg-navy-950 border border-white/15 text-white placeholder-slate-500 text-xs focus:outline-none focus:border-gold-400">
                                </div>
                            </div>

                            <!-- Nama Pemesan (Opsional) -->
                            <div>
                                <input type="text" id="buyerName" placeholder="Nama pemesan (opsional, misal: Rina - SMP)"
                                       class="w-full px-3 py-2 rounded-xl bg-navy-900 border border-white/15 text-white placeholder-slate-500 text-xs focus:outline-none focus:border-gold-400">
                            </div>

                            <!-- Total Harga Real-Time + Tombol Utama WhatsApp -->
                            <div class="pt-2 border-t border-white/10">
                                <div class="flex items-center justify-between mb-2.5 px-1">
                                    <div>
                                        <div class="text-[11px] text-slate-400 font-semibold">Total (<span id="totalSheets" class="text-white font-bold">0</span> lembar)</div>
                                        <div id="deliveryNote" class="text-[10px] text-slate-400">Ambil di Pandu Senjaya RT 12 RW 3</div>
                                    </div>
                                    <div id="totalPrice" class="font-display text-2xl sm:text-3xl font-extrabold text-gold-400">
                                        Rp 0
                                    </div>
                                </div>

                                <button type="submit"
                                        class="w-full py-3 px-4 rounded-xl bg-gradient-to-r from-emerald-500 to-emerald-600 hover:from-emerald-400 hover:to-emerald-500 text-white font-extrabold text-xs sm:text-sm shadow-lg shadow-emerald-600/25 flex items-center justify-center gap-2 transition-all active:scale-95">
                                    <i class="fa-brands fa-whatsapp text-lg"></i>
                                    <span>Pesan & Kirim File via WhatsApp</span>
                                </button>
                            </div>
                        </form>
                    </div>
                </section>
            </div>

        </div>
    </main>

    <!-- FOOTER SUPER RINGKAS -->
    <footer class="border-t border-white/10 bg-navy-950/80 py-2.5 px-4 text-center text-[11px] text-slate-400">
        <span class="font-bold text-slate-200">vutaa print</span> • Desa Pandu Senjaya RT 12 RW 3, SP 4 Pangkalan Lada • WA: 0858-2452-2033
    </footer>

    <!-- SCRIPT LOGIKA KALKULATOR, QR CODE & WHATSAPP -->
    <script>
        const PRICE_UNIT = 1000;
        const WA_PHONE = "6285824522033";
        const DISPLAY_PHONE = "0858-2452-2033";

        // Generate QR Code WhatsApp saat halaman dimuat
        window.addEventListener("DOMContentLoaded", () => {
            try {
                const waDirectLink = `https://wa.me/${WA_PHONE}?text=${encodeURIComponent("Halo vutaa print, saya mau order print dokumen.")}`;
                new QRCode(document.getElementById("qrcode"), {
                    text: waDirectLink,
                    width: 112,
                    height: 112,
                    colorDark: "#0B132B",
                    colorLight: "#FFFFFF",
                    correctLevel: QRCode.CorrectLevel.H
                });
            } catch (err) {
                console.error("QR Error:", err);
            }
            recalculate();
        });

        function formatIDR(num) {
            return "Rp " + num.toLocaleString("id-ID");
        }

        function updateQty(id, delta) {
            const el = document.getElementById(id);
            const current = parseInt(el.value) || 0;
            el.value = Math.max(0, current + delta);
            recalculate();
        }

        function resetCalculator() {
            document.getElementById("qtyBw").value = 0;
            document.getElementById("qtyColor").value = 0;
            document.getElementById("qtyFull").value = 0;
            document.getElementById("buyerName").value = "";
            document.getElementById("deliveryAddress").value = "";
            document.querySelector('input[name="method"][value="Ambil di Tempat"]').checked = true;
            handleMethodChange();
        }

        function handleMethodChange() {
            const method = document.querySelector('input[name="method"]:checked').value;
            const deliverySection = document.getElementById("deliverySection");
            if (method === "Gratis Delivery") {
                deliverySection.classList.remove("hidden");
            } else {
                deliverySection.classList.add("hidden");
            }
            recalculate();
        }

        function recalculate() {
            const bw = Math.max(0, parseInt(document.getElementById("qtyBw").value) || 0);
            const color = Math.max(0, parseInt(document.getElementById("qtyColor").value) || 0);
            const full = Math.max(0, parseInt(document.getElementById("qtyFull").value) || 0);

            const totalSheets = bw + color + full;
            const totalCost = totalSheets * PRICE_UNIT;

            document.getElementById("totalSheets").textContent = totalSheets;
            document.getElementById("totalPrice").textContent = formatIDR(totalCost);

            const method = document.querySelector('input[name="method"]:checked').value;
            const deliveryNote = document.getElementById("deliveryNote");
            const deliveryAlert = document.getElementById("deliveryAlert");

            if (method === "Ambil di Tempat") {
                deliveryNote.textContent = "Ambil di Pandu Senjaya RT 12 RW 3";
                deliveryNote.className = "text-[10px] text-slate-400";
            } else {
                if (totalSheets >= 15) {
                    deliveryNote.textContent = "Gratis Delivery SP 4 (16.30 - 20.00)";
                    deliveryNote.className = "text-[10px] text-emerald-400 font-bold";

                    deliveryAlert.className = "text-[11px] font-semibold px-2.5 py-1.5 rounded-lg bg-emerald-500/20 text-emerald-300 border border-emerald-400/30 leading-snug";
                    deliveryAlert.innerHTML = `<i class="fa-solid fa-circle-check mr-1"></i>Syarat terpenuhi (${totalSheets} lbr)! Gratis antar area SP 4 Pangkalan Lada jam 16.30 - 20.00.`;
                } else {
                    const kurang = 15 - totalSheets;
                    deliveryNote.textContent = `Kurang ${kurang} lbr untuk Gratis Delivery`;
                    deliveryNote.className = "text-[10px] text-amber-400 font-bold";

                    deliveryAlert.className = "text-[11px] font-semibold px-2.5 py-1.5 rounded-lg bg-amber-500/20 text-amber-300 border border-amber-400/30 leading-snug";
                    deliveryAlert.innerHTML = `<i class="fa-solid fa-triangle-exclamation mr-1"></i>Kurang <strong>${kurang} lembar</strong> lagi untuk Gratis Delivery (Min. 15 lbr, area SP 4 Pangkalan Lada, jam 16.30 - 20.00).`;
                }
            }
        }

        document.getElementById("quickOrderForm").addEventListener("submit", function(e) {
            e.preventDefault();

            const bw = Math.max(0, parseInt(document.getElementById("qtyBw").value) || 0);
            const color = Math.max(0, parseInt(document.getElementById("qtyColor").value) || 0);
            const full = Math.max(0, parseInt(document.getElementById("qtyFull").value) || 0);
            const totalSheets = bw + color + full;
            const totalCost = totalSheets * PRICE_UNIT;

            if (totalSheets === 0) {
                showToast("Masukkan minimal 1 lembar dokumen dulu ya!", true);
                return;
            }

            const method = document.querySelector('input[name="method"]:checked').value;
            const address = document.getElementById("deliveryAddress").value.trim();
            const buyerName = document.getElementById("buyerName").value.trim();

            if (method === "Gratis Delivery" && totalSheets < 15) {
                showToast("Gratis Delivery minimal 15 lembar (Area SP 4 Pangkalan Lada).", true);
                return;
            }

            if (method === "Gratis Delivery" && !address) {
                showToast("Tulis alamat/patokan antar di area SP 4 Pangkalan Lada ya!", true);
                document.getElementById("deliveryAddress").focus();
                return;
            }

            let text = `Halo *vutaa print*, saya mau order print:\n`;
            if (buyerName) text += `• Nama: *${buyerName}*\n`;
            text += `\n*Rincian Cetak (Serba 1K):*\n`;
            if (bw > 0) text += `• Dokumen Hitam Putih: ${bw} lbr (${formatIDR(bw * 1000)})\n`;
            if (color > 0) text += `• Berwarna: ${color} lbr (${formatIDR(color * 1000)})\n`;
            if (full > 0) text += `• Full Warna: ${full} lbr (${formatIDR(full * 1000)})\n`;
            text += `• Total: *${totalSheets} lembar — ${formatIDR(totalCost)}*\n\n`;
            text += `*Metode:* ${method}\n`;
            if (method === "Gratis Delivery") {
                text += `• Alamat Antar (SP 4): ${address}\n`;
                text += `• Jadwal Delivery: Jam 16.30 - 20.00\n`;
            }
            text += `\n_File dokumen segera saya kirim setelah pesan ini._`;

            const url = `https://wa.me/${WA_PHONE}?text=${encodeURIComponent(text)}`;
            window.open(url, "_blank", "noopener,noreferrer");
        });

        function copyPhone() {
            const temp = document.createElement("input");
            temp.value = DISPLAY_PHONE;
            document.body.appendChild(temp);
            temp.select();
            try {
                document.execCommand("copy");
                showToast(`Nomor ${DISPLAY_PHONE} berhasil disalin!`);
            } catch (e) {
                showToast("Gagal menyalin nomor.", true);
            }
            document.body.removeChild(temp);
        }

        let toastTimer;
        function showToast(msg, isWarning = false) {
            const toast = document.getElementById("toast");
            const box = document.getElementById("toast-box");
            const icon = document.getElementById("toast-icon");
            const text = document.getElementById("toast-message");

            text.textContent = msg;
            if (isWarning) {
                box.className = "bg-brandOrange-600 text-white px-4 py-2.5 rounded-xl shadow-2xl flex items-center gap-2.5 border border-amber-300/40 text-xs font-bold";
                icon.className = "fa-solid fa-triangle-exclamation text-base";
            } else {
                box.className = "bg-emerald-600 text-white px-4 py-2.5 rounded-xl shadow-2xl flex items-center gap-2.5 border border-emerald-400/30 text-xs font-bold";
                icon.className = "fa-solid fa-circle-check text-base";
            }

            toast.classList.remove("translate-y-20", "opacity-0");
            clearTimeout(toastTimer);
            toastTimer = setTimeout(() => {
                toast.classList.add("translate-y-20", "opacity-0");
            }, 3200);
        }
    </script>
</body>
</html>
```
