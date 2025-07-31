<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lapor Bullying - Pusat Pengaduan Sekolah</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f0f9ff;
        }
        .hero-gradient {
            background: linear-gradient(135deg, #3b82f6 0%, #93c5fd 100%);
        }
        .form-container {
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .confirmation-modal {
            transition: all 0.3s ease;
        }
        .animate-bounce {
            animation: bounce 1s infinite;
        }
        @keyframes bounce {
            0%, 100% {
                transform: translateY(-5px);
            }
            50% {
                transform: translateY(5px);
            }
        }
        .floating-button {
            box-shadow: 0 4px 14px 0 rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="bg-white shadow-md">
        <div class="max-w-6xl mx-auto px-4">
            <div class="flex justify-between items-center py-4">
                <div class="flex items-center space-x-2">
                    <img src="https://placehold.co/40x40" alt="Logo Sekolah dengan simbol perisai dan buku" class="w-10 h-10 rounded-full">
                    <span class="text-xl font-semibold text-blue-600">LaporBK</span>
                </div>
                <div class="hidden md:flex space-x-8">
                    <a href="#about" class="text-gray-600 hover:text-blue-600">Tentang Kami</a>
                    <a href="#procedure" class="text-gray-600 hover:text-blue-600">Prosedur</a>
                    <a href="#faq" class="text-gray-600 hover:text-blue-600">FAQ</a>
                    <a href="#contact" class="text-gray-600 hover:text-blue-600">Kontak</a>
                </div>
                <button class="md:hidden" id="mobile-menu-button">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div class="hidden md:hidden bg-white py-2 px-4" id="mobile-menu">
            <a href="#about" class="block py-2 text-gray-600 hover:text-blue-600">Tentang Kami</a>
            <a href="#procedure" class="block py-2 text-gray-600 hover:text-blue-600">Prosedur</a>
            <a href="#faq" class="block py-2 text-gray-600 hover:text-blue-600">FAQ</a>
            <a href="#contact" class="block py-2 text-gray-600 hover:text-blue-600">Kontak</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-gradient text-white py-16 md:py-24">
        <div class="max-w-6xl mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-8 md:mb-0">
                <h1 class="text-3xl md:text-4xl font-bold mb-4">Laporkan Bullying dengan Aman</h1>
                <p class="text-xl mb-6">Platform resmi untuk melaporkan kasus bullying di sekolah Anda secara rahasia dan terjamin.</p>
                <div class="flex flex-wrap gap-3">
                    <a href="#report" class="bg-white text-blue-600 px-6 py-3 rounded-lg font-medium hover:bg-gray-50 transition">Laporkan Sekarang</a>
                    <a href="#procedure" class="border-2 border-white text-white px-6 py-3 rounded-lg font-medium hover:bg-white hover:text-blue-600 transition">Pelajari Prosedur</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="https://placehold.co/500x350" alt="Siswa yang bahagia bermain bersama di lingkungan sekolah yang positif" class="rounded-lg shadow-xl">
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Kenapa Harus Melapor?</h2>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-gray-50 p-6 rounded-lg">
                    <div class="bg-blue-100 w-12 h-12 rounded-full flex items-center justify-center mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15l8-8m0 0l-8-8m8 8H4" />
                        </svg>
                    </div>
                    <h3 class="font-semibold text-lg mb-2 text-gray-800">Respons Cepat</h3>
                    <p class="text-gray-600">Laporan Anda akan segera ditindaklanjuti oleh Guru BK dalam 24 jam setelah pengiriman.</p>
                </div>
                <div class="bg-gray-50 p-6 rounded-lg">
                    <div class="bg-blue-100 w-12 h-12 rounded-full flex items-center justify-center mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 11c0 3.517-1.009 6.799-2.753 9.571m-3.44-2.04l.054-.09A13.916 13.916 0 008 11a4 4 0 118 0c0 1.017-.07 2.019-.203 3m-2.118 6.844A21.88 21.88 0 0015.171 17m3.839 1.132c.645-2.266.99-4.659.99-7.132A8 8 0 008 4.07M3 15.364c.64-1.319 1-2.8 1-4.364 0-1.457.39-2.823 1.07-4" />
                        </svg>
                    </div>
                    <h3 class="font-semibold text-lg mb-2 text-gray-800">Kerahasiaan Terjamin</h3>
                    <p class="text-gray-600">Identitas Anda akan kami rahasiakan. Tidak ada yang tahu siapa yang melapor.</p>
                </div>
                <div class="bg-gray-50 p-6 rounded-lg">
                    <div class="bg-blue-100 w-12 h-12 rounded-full flex items-center justify-center mb-4">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                        </svg>
                    </div>
                    <h3 class="font-semibold text-lg mb-2 text-gray-800">Sistem Pendukung</h3>
                    <p class="text-gray-600">Anda akan mendapatkan pendampingan psikologis jika dibutuhkan setelah laporan dibuat.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Report Form Section -->
    <section id="report" class="py-16 bg-gray-50">
        <div class="max-w-4xl mx-auto px-4">
            <div class="form-container bg-white rounded-xl p-8 md:p-10">
                <h2 class="text-2xl font-bold text-center mb-8 text-gray-800">Formulir Pengaduan Bullying</h2>
                <form id="bullyingReportForm">
                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2" for="reportType">Jenis Pengaduan *</label>
                        <select id="reportType" name="reportType" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" required>
                            <option value="">Pilih jenis pengaduan</option>
                            <option value="verbal">Bullying Verbal (e.g. ejekan, ancaman)</option>
                            <option value="physical">Bullying Fisik</option>
                            <option value="social">Bullying Sosial</option>
                            <option value="cyber">Cyberbullying</option>
                            <option value="other">Lainnya</option>
                        </select>
                    </div>

                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2" for="incidentDate">Tanggal Kejadian *</label>
                        <input type="date" id="incidentDate" name="incidentDate" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" required>
                    </div>

                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2" for="incidentLocation">Lokasi Kejadian *</label>
                        <select id="incidentLocation" name="incidentLocation" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" required>
                            <option value="">Pilih lokasi</option>
                            <option value="classroom">Kelas</option>
                            <option value="schoolyard">Halaman Sekolah</option>
                            <option value="cafeteria">Kantin</option>
                            <option value="bathroom">Kamar Mandi</option>
                            <option value="online">Daring/Online</option>
                            <option value="other">Lainnya</option>
                        </select>
                    </div>

                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2" for="incidentDetails">Detail Kejadian *</label>
                        <textarea id="incidentDetails" name="incidentDetails" rows="5" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" placeholder="Ceritakan apa yang terjadi secara lengkap..." required></textarea>
                    </div>

                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2" for="evidence">Bukti Pendukung (Opsional)</label>
                        <input type="file" id="evidence" name="evidence" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500" multiple>
                        <p class="text-sm text-gray-500 mt-1">Anda dapat mengunggah foto, video, atau dokumen pendukung (maks. 5MB per file)</p>
                    </div>

                    <div class="mb-6">
                        <label class="block text-gray-700 mb-2" for="anonymous">Identitas Diri</label>
                        <div class="space-y-3">
                            <label class="flex items-center space-x-2">
                                <input type="radio" name="anonymous" value="yes" checked class="form-radio text-blue-600">
                                <span>Saya ingin tetap anonim</span>
                            </label>
                            <label class="flex items-center space-x-2">
                                <input type="radio" name="anonymous" value="no" class="form-radio text-blue-600">
                                <span>Saya bersedia memberikan identitas</span>
                            </label>
                        </div>
                    </div>

                    <div id="identityFields" class="hidden">
                        <div class="grid md:grid-cols-2 gap-6 mb-6">
                            <div>
                                <label class="block text-gray-700 mb-2" for="fullName">Nama Lengkap</label>
                                <input type="text" id="fullName" name="fullName" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500">
                            </div>
                            <div>
                                <label class="block text-gray-700 mb-2" for="class">Kelas</label>
                                <input type="text" id="class" name="class" class="w-full px-4 py-2 border rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500">
                            </div>
                        </div>
                    </div>

                    <div class="flex items-center mb-6">
                        <input type="checkbox" id="confirmation" name="confirmation" class="form-checkbox h-5 w-5 text-blue-600" required>
                        <label for="confirmation" class="ml-2 text-gray-700">Saya menyatakan bahwa informasi yang diberikan adalah benar *</label>
                    </div>

                    <button type="submit" class="w-full bg-blue-600 text-white py-3 px-6 rounded-lg font-medium hover:bg-blue-700 transition focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2">
                        Kirim Laporan
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Procedure Section -->
    <section id="procedure" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12 text-gray-800">Prosedur Penanganan Laporan</h2>
            <div class="relative">
                <!-- Timeline -->
                <div class="hidden md:block absolute left-1/2 h-full w-1 bg-blue-200 transform -translate-x-1/2"></div>
                
                <!-- Timeline Items -->
                <div class="relative z-10 space-y-8 md:space-y-0">
                    <!-- Item 1 -->
                    <div class="flex flex-col md:flex-row items-center md:items-start mb-8">
                        <div class="flex-shrink-0 bg-blue-600 rounded-full w-12 h-12 flex items-center justify-center text-white font-bold mb-4 md:mb-0 md:mr-6">
                            1
                        </div>
                        <div class="md:w-1/2 md:pt-2 md:pr-8">
                            <h3 class="text-xl font-semibold text-blue-600 mb-2">Pengiriman Laporan</h3>
                            <p class="text-gray-600">Murid mengisi formulir pengaduan secara online dengan detail yang jelas.</p>
                        </div>
                        <div class="hidden md:block md:w-1/2"></div>
                    </div>

                    <!-- Item 2 -->
                    <div class="flex flex-col md:flex-row items-center md:items-start mb-8">
                        <div class="hidden md:block md:w-1/2"></div>
                        <div class="flex-shrink-0 bg-blue-600 rounded-full w-12 h-12 flex items-center justify-center text-white font-bold mb-4 md:mb-0 md:ml-6 md:order-last">
                            2
                        </div>
                        <div class="md:w-1/2 md:pt-2 md:pl-8 md:text-right">
                            <h3 class="text-xl font-semibold text-blue-600 mb-2">Verifikasi Laporan</h3>
                            <p class="text-gray-600">Guru BK menerima laporan dan melakukan verifikasi awal dalam 24 jam.</p>
                        </div>
                    </div>

                    <!-- Item 3 -->
                    <div class="flex flex-col md:flex-row items-center md:items-start mb-8">
                        <div class="flex-shrink-0 bg-blue-600 rounded-full w-12 h-12 flex items-center justify-center text-white font-bold mb-4 md:mb-0 md:mr-6">
                            3
                        </div>
                        <div class="md:w-1/2 md:pt-2 md:pr-8">
                            <h3 class="text-xl font-semibold text-blue-600 mb-2">Penyelidikan</h3>
                            <p class="text-gray-600">Tim BK melakukan penyelidikan lebih lanjut dan mengumpulkan bukti pendukung.</p>
                        </div>
                        <div class="hidden md:block md:w-1/2"></div>
                    </div>

                    <!-- Item 4 -->
                    <div class="flex flex-col md:flex-row items-center md:items-start mb-8">
                        <div class="hidden md:block md:w-1/2"></div>
                        <div class="flex-shrink-0 bg-blue-600 rounded-full w-12 h-12 flex items-center justify-center text-white font-bold mb-4 md:mb-0 md:ml-6 md:order-last">
                            4
                        </div>
                        <div class="md:w-1/2 md:pt-2 md:pl-8 md:text-right">
                            <h3 class="text-xl font-semibold text-blue-600 mb-2">Intervensi</h3>
                            <p class="text-gray-600">Memberikan pendampingan pada korban dan penanganan terhadap pelaku bullying.</p>
                        </div>
                    </div>

                    <!-- Item 5 -->
                    <div class="flex flex-col md:flex-row items-center md:items-start">
                        <div class="flex-shrink-0 bg-blue-600 rounded-full w-12 h-12 flex items-center justify-center text-white font-bold mb-4 md:mb-0 md:mr-6">
                            5
                        </div>
                        <div class="md:w-1/2 md
.
