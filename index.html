<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplikasi Daur Ulang</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome CDN for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <!-- Inter font from Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <!-- Babel for JSX transformation in browser (for development only) -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <!-- React and ReactDOM CDNs -->
    <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>

    <style>
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            background-color: #f8fafc; /* Tailwind gray-50 equivalent */
        }
        @keyframes scan-line {
            0% { top: 0%; }
            50% { top: 99%; }
            100% { top: 0%; }
        }
        .animate-scan-line {
            animation: scan-line 3s infinite linear;
        }
        /* Custom Tailwind-like colors/shadows if not directly available or for consistency */
        .bg-green-50 { background-color: #f0fdf4; }
        .text-green-600 { color: #16a34a; }
        .bg-green-500 { background-color: #22c55e; }
        .bg-green-600 { background-color: #16a34a; }
        .hover\:bg-green-700:hover { background-color: #15803d; }
        .text-yellow-500 { color: #f59e0b; }
        .bg-yellow-500 { background-color: #f59e0b; }
        .hover\:bg-yellow-600:hover { background-color: #d97706; }
        .bg-blue-500 { background-color: #3b82f6; }
        .hover\:bg-blue-600:hover { background-color: #2563eb; }
        .bg-purple-500 { background-color: #a855f7; }
        .hover\:bg-purple-600:hover { background-color: #9333ea; }
        .rounded-t-3xl { border-top-left-radius: 1.5rem; border-top-right-radius: 1.5rem; }
        .rounded-b-2xl { border-bottom-left-radius: 1rem; border-bottom-right-radius: 1rem; }
        .rounded-2xl { border-radius: 1rem; }
        .rounded-xl { border-radius: 0.75rem; }
        .shadow-md { box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06); }
        .shadow-lg { box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05); }
        .shadow-xl { box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04); }
        .transition-all { transition-property: all; transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1); transition-duration: 150ms; }
        .duration-300 { transition-duration: 300ms; }
        .transform { transform: var(--tw-transform); }
        .hover\:scale-105:hover { --tw-scale-x: 1.05; --tw-scale-y: 1.05; transform: var(--tw-transform); }
        .hover\:shadow-lg:hover { box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05); }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        // React application code goes here
        const { useState, useEffect } = React;

        // Main App component
        const App = () => {
            // State to manage current screen/page, now defaults to 'scan-qr'
            const [currentScreen, setCurrentScreen] = useState('scan-qr'); // Changed to 'scan-qr'
            // State to simulate points
            const [points, setPoints] = useState(1250);
            // State to simulate loading for scanning
            const [isScanning, setIsScanning] = useState(false);
            // State for search input in "Find Machine"
            const [searchQuery, setSearchQuery] = useState('');

            // Function to navigate between screens
            const navigateTo = (screenName) => {
                setCurrentScreen(screenName);
                // Scroll to top when navigating
                window.scrollTo(0, 0);
            };

            // Simulate scanning process
            const handleScan = () => {
                setIsScanning(true);
                // Simulate API call or processing time
                setTimeout(() => {
                    setPoints(prevPoints => prevPoints + 100); // Add 100 points
                    setIsScanning(false);
                    alert('Pemindaian selesai! Anda mendapatkan 100 poin.');
                    navigateTo('home'); // Go back to home after scan
                }, 3000); // 3 seconds simulation
            };

            // Placeholder for a custom alert/modal instead of window.alert
            const alert = (message) => {
                // In a real app, you'd render a modal here
                console.log("ALERT:", message);
                const modal = document.createElement('div');
                modal.className = 'fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50';
                modal.innerHTML = `
                    <div class="bg-white p-6 rounded-lg shadow-xl max-w-sm mx-auto text-center">
                        <p class="text-lg font-semibold mb-4">${message}</p>
                        <button id="close-modal" class="bg-green-600 hover:bg-green-700 text-white font-bold py-2 px-4 rounded-full">Tutup</button>
                    </div>
                `;
                document.body.appendChild(modal);
                document.getElementById('close-modal').onclick = () => {
                    document.body.removeChild(modal);
                };
            };

            // Component for the Header
            const Header = ({ title, showBackButton = false, onBack = () => {} }) => (
                <div className="flex items-center justify-between p-4 bg-white shadow-sm rounded-b-xl">
                    {showBackButton ? (
                        <button onClick={onBack} className="text-gray-600 text-2xl">
                            <i className="fas fa-arrow-left"></i>
                        </button>
                    ) : (
                        <div className="text-xl font-semibold text-gray-800">10.00</div>
                    )}
                    <div className="flex items-center space-x-2">
                        <i className="fas fa-signal text-gray-600"></i>
                        <i className="fas fa-wifi text-gray-600"></i>
                        <i className="fas fa-battery-full text-gray-600"></i>
                    </div>
                </div>
            );

            // Component for the Bottom Navigation Bar
            const BottomNavBar = () => (
                <div className="fixed bottom-0 left-0 right-0 bg-white shadow-lg p-3 flex justify-around items-center rounded-t-3xl border-t border-gray-200 z-40">
                    <button onClick={() => navigateTo('home')} className={`flex flex-col items-center p-2 rounded-full transition-colors duration-200 ${currentScreen === 'home' ? 'text-green-600 bg-green-50' : 'text-gray-500'}`}>
                        <i className="fas fa-th-large text-xl"></i>
                        <span className="text-xs mt-1">Beranda</span>
                    </button>
                    <button onClick={() => navigateTo('scan-qr')} className={`relative -top-4 bg-green-500 p-4 rounded-full shadow-lg transition-colors duration-200 ${currentScreen === 'scan-qr' ? 'bg-green-600' : 'bg-green-500'} text-white`}>
                        <i className="fas fa-qrcode text-2xl"></i>
                    </button>
                    <button onClick={() => navigateTo('find-machine')} className={`flex flex-col items-center p-2 rounded-full transition-colors duration-200 ${currentScreen === 'find-machine' ? 'text-green-600 bg-green-50' : 'text-gray-500'}`}>
                        <i className="fas fa-search text-xl"></i>
                        <span className="text-xs mt-1">Cari</span>
                    </button>
                    <button onClick={() => navigateTo('learn')} className={`flex flex-col items-center p-2 rounded-full transition-colors duration-200 ${currentScreen === 'learn' ? 'text-green-600 bg-green-50' : 'text-gray-500'}`}>
                        <i className="fas fa-book-open text-xl"></i>
                        <span className="text-xs mt-1">Edukasi</span>
                    </button>
                    <button onClick={() => navigateTo('marketplace')} className={`flex flex-col items-center p-2 rounded-full transition-colors duration-200 ${currentScreen === 'marketplace' ? 'text-green-600 bg-green-50' : 'text-gray-500'}`}>
                        <i className="fas fa-store text-xl"></i>
                        <span className="text-xs mt-1">Toko</span>
                    </button>
                </div>
            );

            // Home Screen Component
            const HomeScreen = () => (
                <div className="p-4 pt-0 bg-gray-50 min-h-screen pb-20">
                    {/* User Profile and Points Section */}
                    <div className="flex justify-between items-center py-4 px-2 rounded-b-2xl">
                        <div className="flex items-center space-x-3">
                            <img
                                src="https://placehold.co/60x60/808080/FFFFFF?text=Adam" // Placeholder for profile image
                                alt="User Profile"
                                className="w-14 h-14 rounded-full border-2 border-green-500 shadow-md"
                                onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/60x60/808080/FFFFFF?text=User"; }}
                            />
                            <div>
                                <p className="text-gray-700 text-sm">Selamat Datang,</p>
                                <p className="font-bold text-lg text-gray-900">Adam</p>
                            </div>
                        </div>
                        <div className="flex items-center bg-white px-4 py-2 rounded-full shadow-md">
                            <i className="fas fa-coins text-yellow-500 text-lg mr-2"></i>
                            <span className="font-semibold text-gray-800">{points} Poin</span>
                        </div>
                    </div>

                    {/* Header image with trees */}
                    <div className="relative w-full h-48 bg-gradient-to-br from-green-100 to-lime-50 rounded-3xl overflow-hidden shadow-lg mb-6">
                        <img
                            src="https://placehold.co/300x150/dcfce7/16a34a?text=Trees"
                            alt="Decorative trees"
                            className="absolute bottom-0 left-0 w-full h-full object-cover opacity-60 rounded-3xl"
                            onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/300x150/dcfce7/16a34a?text=Trees"; }}
                        />
                        <div className="absolute inset-0 flex items-center justify-center">
                            <div className="bg-white bg-opacity-80 px-6 py-3 rounded-full shadow-md text-green-700 font-semibold text-sm animate-pulse">
                                Siklus Hidup: <span className="font-bold">00:00</span>
                            </div>
                        </div>
                    </div>

                    {/* Action Cards */}
                    <div className="space-y-4">
                        {/* Scan & Collect Points Card */}
                        <div className="bg-white p-5 rounded-2xl shadow-md flex items-center space-x-4 hover:shadow-lg transition-shadow duration-300">
                            <div className="w-20 h-20 flex-shrink-0">
                                <img
                                    src="https://placehold.co/80x80/d9f991/166534?text=Scan"
                                    alt="Scan Icon"
                                    className="w-full h-full object-contain"
                                    onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/80x80/d9f991/166534?text=Scan"; }}
                                />
                            </div>
                            <div>
                                <h3 className="font-bold text-lg text-gray-800">Pindai & Kumpulkan Poin</h3>
                                <p className="text-gray-600 text-sm mt-1">Pindai barcode mesin untuk dapatkan poin instan.</p>
                                <button
                                    onClick={() => navigateTo('scan-qr')}
                                    className="mt-3 bg-yellow-500 hover:bg-yellow-600 text-white font-bold py-2 px-4 rounded-full shadow-md transition-all duration-300 transform hover:scale-105"
                                >
                                    Mulai Pindai <i className="fas fa-barcode ml-2"></i>
                                </button>
                            </div>
                        </div>

                        {/* Find Nearby Machine Card */}
                        <div className="bg-white p-5 rounded-2xl shadow-md flex items-center space-x-4 hover:shadow-lg transition-shadow duration-300">
                            <div className="w-20 h-20 flex-shrink-0">
                                <img
                                    src="https://placehold.co/80x80/a7f3d0/065f46?text=Map"
                                    alt="Map Icon"
                                    className="w-full h-full object-contain"
                                    onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/80x80/a7f3d0/065f46?text=Map"; }}
                                />
                            </div>
                            <div>
                                <h3 className="font-bold text-lg text-gray-800">Temukan Mesin Terdekat</h3>
                                <p className="text-gray-600 text-sm mt-1">GPS akan tunjukkan rute & jarak.</p>
                                <button
                                    onClick={() => navigateTo('find-machine')}
                                    className="mt-3 bg-green-600 hover:bg-green-700 text-white font-bold py-2 px-4 rounded-full shadow-md transition-all duration-300 transform hover:scale-105"
                                >
                                    Mulai Temukan <i className="fas fa-map-marker-alt ml-2"></i>
                                </button>
                            </div>
                        </div>

                        {/* Learn Recycling Card */}
                        <div className="bg-white p-5 rounded-2xl shadow-md flex items-center space-x-4 hover:shadow-lg transition-shadow duration-300">
                            <div className="w-20 h-20 flex-shrink-0">
                                <img
                                    src="https://placehold.co/80x80/bfdbfe/1e40af?text=Learn"
                                    alt="Learn Icon"
                                    className="w-full h-full object-contain"
                                    onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/80x80/bfdbfe/1e40af?text=Learn"; }}
                                />
                            </div>
                            <div>
                                <h3 className="font-bold text-lg text-gray-800">Belajar Daur Ulang</h3>
                                <p className="text-gray-600 text-sm mt-1">Pelajari cara memilih & olah sampah jadi produk.</p>
                                <button
                                    onClick={() => navigateTo('learn')}
                                    className="mt-3 bg-blue-500 hover:bg-blue-600 text-white font-bold py-2 px-4 rounded-full shadow-md transition-all duration-300 transform hover:scale-105"
                                >
                                    Mulai Belajar <i className="fas fa-lightbulb ml-2"></i>
                                </button>
                            </div>
                        </div>

                        {/* Marketplace Card */}
                        <div className="bg-white p-5 rounded-2xl shadow-md flex items-center space-x-4 hover:shadow-lg transition-shadow duration-300">
                            <div className="w-20 h-20 flex-shrink-0">
                                <img
                                    src="https://placehold.co/80x80/fef08a/854d0e?text=Shop"
                                    alt="Shop Icon"
                                    className="w-full h-full object-contain"
                                    onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/80x80/fef08a/854d0e?text=Shop"; }}
                                />
                            </div>
                            <div>
                                <h3 className="font-bold text-lg text-gray-800">Marketplace Poin</h3>
                                <p className="text-gray-600 text-sm mt-1">Tukar poinmu dengan produk daur ulang, atau jual hasil kreasimu!</p>
                                <button
                                    onClick={() => navigateTo('marketplace')}
                                    className="mt-3 bg-purple-500 hover:bg-purple-600 text-white font-bold py-2 px-4 rounded-full shadow-md transition-all duration-300 transform hover:scale-105"
                                >
                                    Kunjungi Marketplace <i className="fas fa-shopping-bag ml-2"></i>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            );

            // Scan QR Screen Component
            const ScanQRScreen = () => (
                <div className="flex flex-col items-center p-4 bg-gray-100 min-h-screen pb-20">
                    <Header showBackButton={true} onBack={() => navigateTo('home')} />
                    <div className="flex-grow flex flex-col items-center justify-center w-full max-w-lg mx-auto p-6 bg-white rounded-3xl shadow-xl border border-green-200">
                        <h2 className="text-3xl font-extrabold text-green-700 mb-6 text-center">
                            Pindai Barcode Mesin Daur Ulang
                        </h2>
                        <p className="text-gray-600 mb-8 text-center text-lg leading-relaxed">
                            Arahkan kamera Anda ke barcode yang tersedia pada mesin untuk memulai proses daur ulang.
                        </p>

                        <div className="relative w-72 h-72 border-4 border-dashed border-green-500 rounded-2xl flex items-center justify-center overflow-hidden bg-gradient-to-br from-green-50 to-white shadow-inner">
                            {/* Visual scanner animation */}
                            <div className="absolute inset-0 flex items-center justify-center">
                                <i className="fas fa-camera text-green-300 text-9xl opacity-40"></i>
                            </div>
                            <div className="absolute w-full h-1 bg-green-500 animate-scan-line z-10"></div>
                            {/* Scanner corners */}
                            <div className="absolute top-0 left-0 w-8 h-8 border-t-4 border-l-4 border-green-600 rounded-tl-lg"></div>
                            <div className="absolute top-0 right-0 w-8 h-8 border-t-4 border-r-4 border-green-600 rounded-tr-lg"></div>
                            <div className="absolute bottom-0 left-0 w-8 h-8 border-b-4 border-l-4 border-green-600 rounded-bl-lg"></div>
                            <div className="absolute bottom-0 right-0 w-8 h-8 border-b-4 border-r-4 border-green-600 rounded-bl-lg"></div>
                        </div>

                        <button
                            onClick={handleScan}
                            disabled={isScanning}
                            className={`mt-10 px-8 py-4 rounded-full font-bold text-white shadow-lg transition-all duration-300 transform ${isScanning ? 'bg-gray-400 cursor-not-allowed' : 'bg-green-600 hover:bg-green-700 hover:scale-105'} flex items-center justify-center`}
                        >
                            {isScanning ? (
                                <>
                                    <i className="fas fa-spinner fa-spin mr-3 text-xl"></i> Memindai...
                                </>
                            ) : (
                                <>
                                    <i className="fas fa-camera-retro mr-3 text-xl"></i> Mulai Pindai
                                </>
                            )}
                        </button>
                    </div>
                </div>
            );

            // Find Machine Screen Component
            const FindMachineScreen = () => (
                <div className="flex flex-col p-4 bg-gray-50 min-h-screen pb-20">
                    <Header showBackButton={true} onBack={() => navigateTo('home')} />
                    <div className="flex-grow flex flex-col items-center pt-8 w-full max-w-md mx-auto">
                        <h2 className="text-2xl font-bold text-gray-800 mb-8 text-center">Cari Trash Vending Machine Terdekat</h2>

                        <button
                            onClick={() => alert('Mencari mesin terdekat menggunakan GPS Anda... (Fitur ini akan terhubung ke API lokasi sungguhan)')}
                            className="bg-green-600 hover:bg-green-700 text-white font-bold py-3 px-6 rounded-full shadow-lg transition-all duration-300 transform hover:scale-105 mb-8 flex items-center justify-center"
                        >
                            <i className="fas fa-location-arrow mr-3 text-lg"></i> Temukan Mesin Terdekat
                        </button>

                        <div className="relative w-full mb-6">
                            <input
                                type="text"
                                placeholder="Cari kota atau kecamatan..."
                                value={searchQuery}
                                onChange={(e) => setSearchQuery(e.target.value)}
                                className="w-full p-4 pl-12 pr-4 rounded-full bg-white border border-gray-300 shadow-md focus:outline-none focus:ring-2 focus:ring-green-500 text-gray-800"
                            />
                            <i className="fas fa-search absolute left-4 top-1/2 -translate-y-1/2 text-gray-400"></i>
                            {searchQuery && (
                                <button
                                    onClick={() => setSearchQuery('')}
                                    className="absolute right-4 top-1/2 -translate-y-1/2 text-gray-500 hover:text-gray-700"
                                >
                                    <i className="fas fa-times-circle"></i>
                                </button>
                            )}
                        </div>

                        <div className="w-full text-center text-gray-500 text-sm mt-4">
                            {searchQuery ? `Hasil pencarian untuk "${searchQuery}" akan muncul di sini.` : 'Masukkan nama kota atau kecamatan untuk mencari.'}
                        </div>

                        <div className="w-full h-64 bg-gray-200 rounded-xl flex items-center justify-center text-gray-500 mt-6 shadow-inner">
                            {/* Placeholder for map */}
                            <i className="fas fa-map-marked-alt text-6xl"></i>
                            <p className="ml-4">Peta akan ditampilkan di sini</p>
                        </div>
                    </div>
                </div>
            );

            // Learn Screen Component
            const LearnScreen = () => (
                <div className="flex flex-col p-4 bg-gray-50 min-h-screen pb-20">
                    <Header showBackButton={true} onBack={() => navigateTo('home')} />
                    <div className="flex-grow flex flex-col items-center pt-8 w-full max-w-md mx-auto">
                        <h2 className="text-3xl font-bold text-gray-800 mb-8 text-center">Belajar Daur Ulang</h2>

                        <div className="bg-white p-6 rounded-2xl shadow-lg mb-6 w-full transform transition-transform duration-300 hover:scale-[1.02]">
                            <h3 className="font-bold text-xl text-green-700 mb-3">Memilah Sampah dengan Benar</h3>
                            <p className="text-gray-700 text-base leading-relaxed">
                                Memilah sampah adalah langkah pertama yang krusial. Kenali jenis-jenis sampah seperti plastik, kertas, kaca, dan organik. Pastikan sampah bersih sebelum dibuang ke tempat yang sesuai.
                            </p>
                            <button onClick={() => alert('Membuka materi lebih lanjut tentang pemilahan sampah...')} className="mt-4 text-blue-600 hover:underline font-semibold">
                                Baca Selengkapnya <i className="fas fa-arrow-right ml-1"></i>
                            </button>
                        </div>

                        <div className="bg-white p-6 rounded-2xl shadow-lg mb-6 w-full transform transition-transform duration-300 hover:scale-[1.02]">
                            <h3 className="font-bold text-xl text-yellow-700 mb-3">Manfaat Daur Ulang</h3>
                            <p className="text-gray-700 text-base leading-relaxed">
                                Daur ulang mengurangi polusi, menghemat energi, dan melestarikan sumber daya alam. Ini adalah kontribusi nyata untuk bumi yang lebih hijau dan masa depan yang berkelanjutan.
                            </p>
                            <button onClick={() => alert('Membuka materi lebih lanjut tentang manfaat daur ulang...')} className="mt-4 text-blue-600 hover:underline font-semibold">
                                Baca Selengkapnya <i className="fas fa-arrow-right ml-1"></i>
                            </button>
                        </div>

                        <div className="bg-white p-6 rounded-2xl shadow-lg mb-6 w-full transform transition-transform duration-300 hover:scale-[1.02]">
                            <h3 className="font-bold text-xl text-purple-700 mb-3">Proyek Daur Ulang Kreatif</h3>
                            <p className="text-gray-700 text-base leading-relaxed">
                                Ubah barang bekas menjadi sesuatu yang baru! Botol plastik bisa jadi pot bunga, kardus jadi tempat pensil, dan kain perca jadi tas belanja. Mari berkreasi!
                            </p>
                            <button onClick={() => alert('Membuka panduan proyek kreatif...')} className="mt-4 text-blue-600 hover:underline font-semibold">
                                Lihat Ide <i className="fas fa-arrow-right ml-1"></i>
                            </button>
                        </div>

                    </div>
                </div>
            );

            // Marketplace Screen Component
            const MarketplaceScreen = () => {
                const products = [
                    { id: 1, name: 'Tas Belanja Daur Ulang', price: 'Rp 45.000', imageUrl: 'https://placehold.co/150x150/fde047/713f12?text=Tas' },
                    { id: 2, name: 'Pot Tanaman dari Botol', price: 'Rp 25.000', imageUrl: 'https://placehold.co/150x150/d9f991/3f6212?text=Pot' },
                    { id: 3, name: 'Buku Catatan Kertas Daur Ulang', price: 'Rp 35.000', imageUrl: 'https://placehold.co/150x150/bfdbfe/172554?text=Buku' },
                    { id: 4, name: 'Tempat Pensil dari Kardus', price: 'Rp 20.000', imageUrl: 'https://placehold.co/150x150/ffe4e6/831843?text=Pensil' },
                ];

                return (
                    <div className="flex flex-col p-4 bg-gray-50 min-h-screen pb-20">
                        <Header showBackButton={true} onBack={() => navigateTo('home')} />
                        <div className="flex-grow flex flex-col items-center pt-8 w-full max-w-md mx-auto">
                            <h2 className="text-3xl font-bold text-gray-800 mb-8 text-center">Marketplace Produk Daur Ulang</h2>

                            <div className="relative w-full h-48 bg-cover bg-center rounded-2xl overflow-hidden shadow-lg mb-6"
                                 style={{ backgroundImage: `url('https://placehold.co/400x200/a7f3d0/065f46?text=Eco+Products')` }}>
                                <div className="absolute inset-0 bg-black bg-opacity-40 flex items-center justify-center">
                                    <h3 className="text-white text-2xl font-bold text-center">
                                        Temukan Produk Unik & Ramah Lingkungan
                                    </h3>
                                </div>
                            </div>

                            <h3 className="text-2xl font-bold text-gray-800 mb-4 self-start">Produk Baru</h3>
                            <div className="grid grid-cols-2 gap-4 w-full">
                                {products.map(product => (
                                    <div key={product.id} className="bg-white rounded-xl shadow-md overflow-hidden transform transition-transform duration-300 hover:scale-105 hover:shadow-lg">
                                        <img
                                            src={product.imageUrl}
                                            alt={product.name}
                                            className="w-full h-32 object-cover"
                                            onError={(e) => { e.target.onerror = null; e.target.src = "https://placehold.co/150x150/cccccc/000000?text=Product"; }}
                                        />
                                        <div className="p-3">
                                            <h4 className="font-semibold text-gray-800 text-base truncate">{product.name}</h4>
                                            <p className="text-green-600 font-bold mt-1">{product.price}</p>
                                            <button
                                                onClick={() => alert(`Anda mengklik ${product.name}. Fitur pembelian belum tersedia.`)}
                                                className="mt-2 bg-green-500 hover:bg-green-600 text-white text-sm py-1 px-3 rounded-full w-full"
                                            >
                                                Beli Sekarang
                                            </button>
                                        </div>
                                    </div>
                                ))}
                            </div>

                            <button
                                onClick={() => alert('Fitur lihat semua produk belum tersedia.')}
                                className="mt-8 bg-blue-500 hover:bg-blue-600 text-white font-bold py-3 px-6 rounded-full shadow-lg transition-all duration-300 transform hover:scale-105"
                            >
                                Lihat Semua Produk <i className="fas fa-arrow-right ml-2"></i>
                            </button>
                        </div>
                    </div>
                );
            };

            // Main render logic based on current screen
            const renderScreen = () => {
                switch (currentScreen) {
                    case 'home':
                        return <HomeScreen />;
                    case 'scan-qr':
                        return <ScanQRScreen />;
                    case 'find-machine':
                        return <FindMachineScreen />;
                    case 'learn':
                        return <LearnScreen />;
                    case 'marketplace':
                        return <MarketplaceScreen />;
                    default:
                        return <HomeScreen />;
                }
            };

            return (
                <div className="relative font-inter antialiased text-gray-900 bg-gray-50">
                    {/* Render the current screen */}
                    <div className="min-h-screen flex flex-col justify-between">
                        <div className="flex-grow">
                            {renderScreen()}
                        </div>
                        {/* Always show the bottom navigation bar */}
                        <BottomNavBar />
                    </div>
                </div>
            );
        };

        // Render the App component into the root div
        ReactDOM.render(<App />, document.getElementById('root'));
    </script>
</body>
</html>
