<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Karyawan - Painting 2W</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script defer src="https://unpkg.com/alpinejs@3.x.x/dist/cdn.min.js"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>[x-cloak] { display: none !important; } body { font-family: 'Plus Jakarta Sans', sans-serif; }</style>
</head>
<body class="bg-slate-50" x-data="appData()" x-init="initApp('data-karyawan')">

    <div class="flex h-screen w-full overflow-hidden">
        <?php include 'layout_sidebar.php'; ?>

        <div class="flex-1 flex flex-col min-w-0 overflow-hidden">
            <header class="bg-white border-b px-8 py-4 flex justify-between items-center z-40">
                <h2 class="text-xl font-extrabold text-slate-800 uppercase">Master Data Karyawan</h2>
                <div class="flex items-center gap-4">
                    <button @click="syncAll()" class="bg-blue-50 text-blue-600 px-4 py-2 rounded-xl font-bold text-xs" 
                            x-text="isSyncing ? 'SINKRON...' : 'REFRESH'"></button>
                </div>
            </header>

            <main class="flex-1 overflow-y-auto p-6 lg:p-10">
                <div class="space-y-6">
                    <div class="bg-white p-6 rounded-[2.5rem] border shadow-sm flex flex-col md:flex-row justify-between items-center gap-4">
                        <div class="relative w-full md:w-96">
                            <i data-lucide="search" class="absolute left-4 top-3 text-slate-400 w-5 h-5"></i>
                            <input type="text" x-model="searchK" placeholder="Cari NIK atau Nama Karyawan..." 
                                   class="w-full pl-12 pr-4 py-3 bg-slate-50 border-2 border-slate-100 rounded-2xl outline-blue-600 font-semibold text-sm transition-all focus:bg-white">
                        </div>
                        <button @click="openModal('karyawan')" class="w-full md:w-auto bg-blue-600 text-white px-8 py-3.5 rounded-2xl font-black text-[10px] uppercase tracking-widest hover:bg-blue-700 transition-all shadow-xl shadow-blue-100">
                            + TAMBAH KARYAWAN
                        </button>
                    </div>

                    <div class="bg-white rounded-[2.5rem] border overflow-hidden shadow-sm">
                        <div class="overflow-x-auto">
                            <table class="w-full text-left border-collapse">
                                <thead class="bg-slate-800 text-white font-bold uppercase text-[10px] tracking-widest">
                                    <tr>
                                        <th class="p-6">NIK Anggota</th>
                                        <th class="p-6">Nama Lengkap</th>
                                        <th class="p-6 text-center">Line / Pos</th>
                                        <th class="p-6 text-center">Status Lapor</th>
                                        <th class="p-6 text-center">Aksi</th>
                                    </tr>
                                </thead>
                                <tbody class="divide-y text-xs font-bold uppercase">
                                    <template x-for="k in filteredK" :key="k.nik">
                                        <tr class="hover:bg-slate-50 transition-colors">
                                            <td class="p-6 text-blue-600 font-black" x-text="k.nik"></td>
                                            <td class="p-6 text-slate-800" x-text="k.nama"></td>
                                            <td class="p-6 text-center text-slate-500" x-text="k.line"></td>
                                            <td class="p-6 text-center">
                                                <template x-if="hasReported(k.nik)">
                                                    <span class="bg-green-100 text-green-600 px-3 py-1.5 rounded-xl inline-flex items-center gap-2">
                                                        <i data-lucide="check-circle-2" class="w-3.5 h-3.5"></i>
                                                        <span class="text-[9px] font-black uppercase">Sudah Lapor</span>
                                                    </span>
                                                </template>
                                                <template x-if="!hasReported(k.nik)">
                                                    <span class="bg-slate-100 text-slate-400 px-3 py-1.5 rounded-xl inline-flex items-center gap-2">
                                                        <i data-lucide="clock-3" class="w-3.5 h-3.5"></i>
                                                        <span class="text-[9px] font-black uppercase tracking-tighter">Belum Lapor</span>
                                                    </span>
                                                </template>
                                            </td>
                                            <td class="p-6 text-center">
                                                <div class="flex gap-2 justify-center">
                                                    <button @click="editKaryawan(k)" class="p-2.5 bg-blue-50 text-blue-600 rounded-xl hover:bg-blue-100 transition-all">
                                                        <i data-lucide="pencil" class="w-4 h-4"></i>
                                                    </button>
                                                    <button @click="deleteData('karyawan', k)" class="p-2.5 bg-red-50 text-red-600 rounded-xl hover:bg-red-100 transition-all">
                                                        <i data-lucide="trash-2" class="w-4 h-4"></i>
                                                    </button>
                                                </div>
                                            </td>
                                        </tr>
                                    </template>
                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>
            </main>
        </div>
    </div>

    <?php include 'layout_modals.php'; ?>
    <?php include 'layout_footer_js.php'; ?>
</body>
</html>
