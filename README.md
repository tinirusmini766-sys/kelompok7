
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IsTY Parfume - Wangi Bikin Menarik</title>
    <!-- Memuat Tailwind CSS dari CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Memuat Font Inter untuk teks utama -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
    <!-- Memuat Font Playful (Cherry Bomb One sebagai pengganti Bubble Pop/Joypops) untuk footer -->
    <link href="https://fonts.googleapis.com/css2?family=Cherry+Bomb+One&display=swap" rel="stylesheet">
    <style>
        /* Mengatur font utama dan font playful */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #ffe6f0; /* Latar belakang pink pastel yang cerah */
            overflow-x: hidden;
            position: relative;
        }

        /* --- Custom Styles & Animations for Theme --- */

        .header-bg {
            background: linear-gradient(135deg, #ffc0d9 0%, #a2d2ff 100%);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .product-card {
            transition: transform 0.3s, box-shadow 0.3s;
            background-color: white;
        }

        .product-card:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 15px 30px rgba(255, 192, 217, 0.5); /* Shadow pink yang menarik */
        }

        /* Animasi Bunga Berjatuhan (Falling Flowers) */
        .flower {
            position: absolute;
            width: 15px;
            height: 15px;
            background-color: #ffb5c5;
            border-radius: 50%;
            opacity: 0.8;
            pointer-events: none;
            animation: fall linear infinite;
        }

        .flower:nth-child(2n) {
            background-color: #ffd8d8;
            width: 12px;
            height: 12px;
            animation-delay: 2s;
            animation-duration: 15s;
        }

        .flower:nth-child(3n) {
            background-color: #a2d2ff;
            width: 18px;
            height: 18px;
            animation-delay: 4s;
            animation-duration: 18s;
        }

        @keyframes fall {
            0% {
                transform: translateY(-100vh) rotate(0deg);
                opacity: 0.5;
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
                opacity: 1;
            }
        }

        /* Konfigurasi untuk 10 bunga */
        .flower-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }

        /* Font khusus footer */
        .footer-font {
            font-family: 'Cherry Bomb One', cursive;
            text-shadow: 2px 2px #fff;
        }

        /* Animasi lucu untuk tombol CTA */
        .cta-button {
            transition: background-color 0.3s, transform 0.2s;
        }
        .cta-button:active {
            transform: scale(0.95);
        }

        /* Style untuk logo pembayaran */
        .payment-logo {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 4px 8px;
            border-radius: 6px;
            font-size: 0.75rem;
            font-weight: 700;
            color: white;
            margin: 2px;
            min-width: 60px;
        }
    </style>
</head>
<body>

    <!-- Animasi Bunga Berjatuhan -->
    <div class="flower-container">
        <div class="flower" style="left: 10%; animation-duration: 12s;"></div>
        <div class="flower" style="left: 20%; animation-duration: 15s; animation-delay: 1s;"></div>
        <div class="flower" style="left: 35%; animation-duration: 10s; animation-delay: 3s;"></div>
        <div class="flower" style="left: 50%; animation-duration: 18s; animation-delay: 5s;"></div>
        <div class="flower" style="left: 65%; animation-duration: 13s; animation-delay: 2s;"></div>
        <div class="flower" style="left: 75%; animation-duration: 16s; animation-delay: 4s;"></div>
        <div class="flower" style="left: 90%; animation-duration: 11s; animation-delay: 0.5s;"></div>
        <div class="flower" style="left: 5%; animation-duration: 14s; animation-delay: 6s;"></div>
        <div class="flower" style="left: 80%; animation-duration: 9s; animation-delay: 1.5s;"></div>
        <div class="flower" style="left: 40%; animation-duration: 17s; animation-delay: 3.5s;"></div>
    </div>
    
    <!-- Header/Hero Section -->
    <header class="header-bg py-20 text-center shadow-lg">
        <div class="container mx-auto px-4">
            <h1 class="text-5xl md:text-7xl font-extrabold text-white mb-2 tracking-tight">
                Wangi kan badan mu dengan parfum roll
            </h1>
            <p class="text-xl md:text-2xl font-semibold text-pink-700 bg-white inline-block px-4 py-2 rounded-full shadow-md mt-4 animate-pulse">
                parfum roll dengan wangi bikin menarik!!
            </p>
        </div>
    </header>

    <!-- Konten Utama: Katalog Produk -->
    <main class="container mx-auto px-4 py-16">
        <h2 class="text-4xl font-bold text-pink-700 text-center mb-12">Pilih Wangi Favoritmu!</h2>
        
        <div id="product-list" class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Kartu Produk 1: Nagita Roll -->
            <div id="nagita-card" class="product-card rounded-xl overflow-hidden shadow-2xl p-6 text-center">
                <img src="https://down-id.img.susercontent.com/file/id-11134207-7r990-lnduo9yi0h9729" onerror="this.onerror=null; this.src='https://placehold.co/300x300/fecaca/9f1239?text=Nagita';" alt="Nagita Roll Parfume" class="w-full h-64 object-cover mb-4 rounded-lg shadow-inner">
                <h3 class="text-3xl font-bold text-pink-600 mb-2">Nagita Roll</h3>
                <p class="text-2xl font-extrabold text-blue-500 mb-4">Rp 7.000</p>
                <p class="text-gray-600 mb-6 italic">Kelembutan Elegan. Aroma yang menghadirkan aura classy dan mahal, cocok untuk Anda yang ingin tampil anggun sepanjang hari. Wanginya tahan lama dan tidak menyengat!</p>
                <a href="#order-form" onclick="prefillQuantity('nagita', 1)" class="cta-button bg-pink-500 hover:bg-pink-600 text-white font-bold py-3 px-8 rounded-full shadow-lg">
                    PESAN SEKARANG
                </a>
            </div>

            <!-- Kartu Produk 2: Sweet Boo Roll -->
            <div id="sweetboo-card" class="product-card rounded-xl overflow-hidden shadow-2xl p-6 text-center">
                <img src="https://down-id.img.susercontent.com/file/id-11134207-7r98s-lnduo9yhw9jv54" onerror="this.onerror=null; this.src='https://placehold.co/300x300/fecaca/9f1239?text=Sweet+Boo';" alt="Sweet Boo Roll Parfume" class="w-full h-64 object-cover mb-4 rounded-lg shadow-inner">
                <h3 class="text-3xl font-bold text-pink-600 mb-2">Sweet Boo Roll</h3>
                <p class="text-2xl font-extrabold text-blue-500 mb-4">Rp 7.500</p>
                <p class="text-gray-600 mb-6 italic">Manis yang Menggoda. Perpaduan wangi fruity dan candy yang ceria dan menggemaskan. Buat hari-hari Anda penuh semangat dan menarik perhatian.</p>
                <a href="#order-form" onclick="prefillQuantity('sweetboo', 1)" class="cta-button bg-pink-500 hover:bg-pink-600 text-white font-bold py-3 px-8 rounded-full shadow-lg">
                    PESAN SEKARANG
                </a>
            </div>

            <!-- Kartu Produk 3: Vanilla Cake Roll -->
            <div id="vanilla-card" class="product-card rounded-xl overflow-hidden shadow-2xl p-6 text-center">
                <img src="https://p16-oec-sg.ibyteimg.com/tos-alisg-i-aphluv4xwc-sg/72a664625a6d427da876d23c1c1c6ca0~tplv-aphluv4xwc-resize-webp:526:525.webp?dr=15592&t=555f072d&ps=933b5bde&shp=8dbd94bf&shcp=e1be8f53&idc=my&from=2378011839" onerror="this.onerror=null; this.src='https://placehold.co/300x300/fecaca/9f1239?text=Vanilla+Cake';" alt="Vanilla Cake Roll Parfume" class="w-full h-64 object-cover mb-4 rounded-lg shadow-inner">
                <h3 class="text-3xl font-bold text-pink-600 mb-2">Vanilla Cake Roll</h3>
                <p class="text-2xl font-extrabold text-blue-500 mb-4">Rp 8.000</p>
                <p class="text-gray-600 mb-6 italic">Kehangatan Dessert. Aroma manis vanilla lembut seperti kue panggang. Wangi yang sangat adiktif, membuat Anda ingin terus menciumnya. Sempurna untuk pecinta wangi manis!</p>
                <a href="#order-form" onclick="prefillQuantity('vanilla', 1)" class="cta-button bg-pink-500 hover:bg-pink-600 text-white font-bold py-3 px-8 rounded-full shadow-lg">
                    PESAN SEKARANG
                </a>
            </div>
        </div>

        <!-- Section Formulir Pemesanan -->
        <section id="order-form" class="mt-20 pt-10 border-t-4 border-dashed border-pink-300">
            <h2 class="text-4xl font-bold text-pink-700 text-center mb-10">Formulir Pemesanan Lengkap</h2>

            <div id="message-box" class="hidden p-4 mb-6 rounded-lg text-center font-semibold transition-all duration-300" role="alert"></div>

            <form id="orderForm" class="bg-white p-8 md:p-12 rounded-2xl shadow-2xl max-w-4xl mx-auto">
                
                <!-- Detail Pemesan -->
                <div class="mb-8 p-4 border-l-4 border-pink-500 bg-pink-50 rounded-lg">
                    <h3 class="text-xl font-bold text-pink-600 mb-4">1. Data Pembeli & Pengiriman</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <input type="text" id="nama" placeholder="Nama Lengkap *" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-pink-500 focus:border-pink-500" required>
                        <input type="tel" id="whatsapp" placeholder="Nomor WhatsApp Aktif (c/o: 628xxxx) *" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-pink-500 focus:border-pink-500" pattern="[0-9+ ]*" title="Hanya angka, spasi, atau simbol plus (+)" required>
                    </div>
                    <textarea id="alamat" placeholder="Alamat Lengkap (Jalan, RT/RW, Kelurahan, Kecamatan) *" rows="3" class="w-full mt-4 p-3 border border-gray-300 rounded-lg focus:ring-pink-500 focus:border-pink-500" required></textarea>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-4">
                        <input type="text" id="kota" placeholder="Kota/Kabupaten *" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-pink-500 focus:border-pink-500" required>
                        <input type="text" id="kodepos" placeholder="Kode Pos" class="w-full p-3 border border-gray-300 rounded-lg focus:ring-pink-500 focus:border-pink-500">
                    </div>
                </div>

                <!-- Detail Pesanan -->
                <div class="mb-8 p-4 border-l-4 border-blue-500 bg-blue-50 rounded-lg">
                    <h3 class="text-xl font-bold text-blue-600 mb-4">2. Pilih Jumlah Produk</h3>
                    <div class="space-y-3">
                        <!-- Nagita Roll -->
                        <div class="flex items-center justify-between bg-white p-3 rounded-lg border">
                            <label for="qty-nagita" class="font-medium text-gray-700">Nagita Roll (Rp 7.000)</label>
                            <input type="number" id="qty-nagita" name="nagita" data-price="7000" min="0" value="0" class="w-20 p-2 border rounded-lg text-center focus:ring-blue-500" onchange="calculateTotal()">
                        </div>
                        <!-- Sweet Boo Roll -->
                        <div class="flex items-center justify-between bg-white p-3 rounded-lg border">
                            <label for="qty-sweetboo" class="font-medium text-gray-700">Sweet Boo Roll (Rp 7.500)</label>
                            <input type="number" id="qty-sweetboo" name="sweetboo" data-price="7500" min="0" value="0" class="w-20 p-2 border rounded-lg text-center focus:ring-blue-500" onchange="calculateTotal()">
                        </div>
                        <!-- Vanilla Cake Roll -->
                        <div class="flex items-center justify-between bg-white p-3 rounded-lg border">
                            <label for="qty-vanilla" class="font-medium text-gray-700">Vanilla Cake Roll (Rp 8.000)</label>
                            <input type="number" id="qty-vanilla" name="vanilla" data-price="8000" min="0" value="0" class="w-20 p-2 border rounded-lg text-center focus:ring-blue-500" onchange="calculateTotal()">
                        </div>
                    </div>
                </div>

                <!-- Total Harga -->
                <div class="mb-8 p-4 bg-yellow-100 rounded-lg shadow-inner flex justify-between items-center">
                    <span class="text-xl font-bold text-yellow-800">TOTAL HARGA PRODUK:</span>
                    <span id="total-price" class="text-3xl font-extrabold text-red-600">Rp 0</span>
                </div>

                <!-- Metode Pembayaran -->
                <div class="mb-8 p-4 border-l-4 border-green-500 bg-green-50 rounded-lg">
                    <h3 class="text-xl font-bold text-green-600 mb-4">3. Metode Pembayaran *</h3>
                    <div class="space-y-3">
                        <!-- Pilihan E-Wallet -->
                        <label class="block">
                            <input type="radio" name="paymentMethod" value="E-Wallet (DANA, GoPay, OVO, ShopeePay)" class="mr-2 text-green-600 focus:ring-green-500" required>
                            E-Wallet (DANA, GoPay, OVO, ShopeePay)
                        </label>
                        <!-- Pilihan QRIS -->
                        <label class="block">
                            <input type="radio" name="paymentMethod" value="QRIS" class="mr-2 text-green-600 focus:ring-green-500">
                            QRIS (Semua Bank/E-Wallet)
                        </label>
                        <!-- Pilihan COD -->
                        <label class="block">
                            <input type="radio" name="paymentMethod" value="Cash / Bayar di Tempat (COD)" class="mr-2 text-green-600 focus:ring-green-500">
                            Cash / Bayar di Tempat (COD)
                        </label>
                    </div>

                    <!-- Logo Pembayaran Kecil -->
                    <div class="mt-4 flex flex-wrap gap-2 justify-center">
                        <span class="payment-logo bg-blue-600">DANA</span>
                        <span class="payment-logo bg-green-500">GoPay</span>
                        <span class="payment-logo bg-purple-600">OVO</span>
                        <span class="payment-logo bg-orange-500">ShopeePay</span>
                        <span class="payment-logo bg-indigo-500">QRIS</span>
                        <span class="payment-logo bg-red-700">COD</span>
                    </div>
                </div>

                <!-- Tombol Submit -->
                <button type="submit" id="submitButton" class="w-full cta-button bg-green-500 hover:bg-green-600 text-white text-2xl font-bold py-4 rounded-xl shadow-lg transform transition duration-200">
                    <span id="submitText">KONFIRMASI PESANAN & KIRIM KE ADMIN VIA WA</span>
                    <span id="loadingSpinner" class="hidden">Memproses...</span>
                </button>
            </form>
        </section>
    </main>

    <!-- Footer -->
    <footer class="mt-20 py-8 text-center bg-pink-400 text-white">
        <div class="container mx-auto px-4">
            <p class="footer-font text-3xl md:text-4xl mb-2">
                IsTY Parfume — Teman Wangi mu!
            </p>
            <p class="text-xs mt-4 text-pink-900 opacity-70">
                di buat oleh kelompok 7 yaitu : nurlisa haerani, tini rusmini, sutan dendira
            </p>
        </div>
    </footer>

    <script>
        // Data Produk
        const products = {
            nagita: { name: "Nagita Roll", price: 7000, qtyId: 'qty-nagita' },
            sweetboo: { name: "Sweet Boo Roll", price: 7500, qtyId: 'qty-sweetboo' },
            vanilla: { name: "Vanilla Cake Roll", price: 8000, qtyId: 'qty-vanilla' }
        };

        const adminWaNumber = '6285891693186'; // Nomor Admin WhatsApp

        // Fungsi untuk memformat angka ke mata uang IDR
        const formatRupiah = (number) => {
            return new Intl.NumberFormat('id-ID', {
                style: 'currency',
                currency: 'IDR',
                minimumFractionDigits: 0
            }).format(number);
        };

        // Fungsi untuk menghitung total harga
        function calculateTotal() {
            let total = 0;
            let totalItem = 0;
            const quantityInputs = document.querySelectorAll('#orderForm input[type="number"]');
            
            quantityInputs.forEach(input => {
                const qty = parseInt(input.value) || 0;
                const price = parseFloat(input.dataset.price);
                total += qty * price;
                totalItem += qty;
            });

            document.getElementById('total-price').textContent = formatRupiah(total);
            return { total, totalItem };
        }

        // Fungsi untuk mengisi kuantitas produk saat tombol CTA diklik
        function prefillQuantity(productId, quantity) {
            // Set semua kuantitas ke 0 dulu
            Object.keys(products).forEach(id => {
                document.getElementById(products[id].qtyId).value = 0;
            });
            
            // Set kuantitas produk yang diklik
            const inputId = products[productId].qtyId;
            document.getElementById(inputId).value = quantity;
            calculateTotal();

            // Opsional: Scroll ke atas form agar pengguna bisa langsung mengisi
            document.getElementById('order-form').scrollIntoView({ behavior: 'smooth' });
        }

        // Fungsi untuk menampilkan pesan (pengganti alert)
        function showMessage(text, type = 'success') {
            const box = document.getElementById('message-box');
            box.textContent = text;
            box.className = 'p-4 mb-6 rounded-lg text-center font-semibold transition-all duration-300';
            
            if (type === 'success') {
                box.classList.add('bg-green-100', 'text-green-700');
            } else if (type === 'error') {
                box.classList.add('bg-red-100', 'text-red-700');
            } else { // info
                box.classList.add('bg-blue-100', 'text-blue-700');
            }
            box.classList.remove('hidden');

            setTimeout(() => {
                box.classList.add('hidden');
            }, 5000);
        }

        // Event listener untuk formulir pemesanan
        document.getElementById('orderForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Mencegah form submission default
            
            const submitButton = document.getElementById('submitButton');
            const submitText = document.getElementById('submitText');
            const loadingSpinner = document.getElementById('loadingSpinner');

            // 1. Validasi Minimum Pesanan
            const { total, totalItem } = calculateTotal();
            if (totalItem === 0) {
                showMessage('Anda harus memilih minimal 1 produk untuk dipesan.', 'error');
                return;
            }

            // 2. Kumpulkan Data Pesanan
            const nama = document.getElementById('nama').value.trim();
            const whatsapp = document.getElementById('whatsapp').value.trim();
            const alamat = document.getElementById('alamat').value.trim();
            const kota = document.getElementById('kota').value.
