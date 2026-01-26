<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Nearmiss - Painting 2W</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script defer src="https://unpkg.com/alpinejs@3.x.x/dist/cdn.min.js"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>[x-cloak] { display: none !important; } body { font-family: 'Plus Jakarta Sans', sans-serif; }</style>
</head>
<body class="bg-slate-50" x-data="appData()" x-init="initApp('data-nearmiss')">

    <div class="flex h-screen w-full overflow-hidden">
        <?php include 'layout_sidebar.php'; ?>

        <div class="flex-1 flex flex-col min-w-0 overflow-hidden">
            <header class="bg-white border-b px-8 py-4 flex justify-between items-center z-40">
                <h2 class="text-xl font-extrabold text-slate-800 uppercase italic">Laporan Nearmiss</h2>
                <div class="flex items-center gap-4">
                    <button @click="syncAll()" class="bg-blue-50 text-blue-600 px-4 py-2 rounded-xl font-bold text-xs" 
                            x-text="isSyncing ? 'SINKRON...' : 'REFRESH'"></button>
                </div>
            </header>

            <main class="flex-1 overflow-y-auto p-6 lg:p-10">
                <div class="space-y-6">
                    <div class="bg-white p-6 rounded-[2.5rem] border shadow-sm flex flex-col md:flex-row gap-4">
                        <div class="relative flex-1">
                            <i data-lucide="search" class="absolute left-4 top-3.5 text-slate-400 w-5 h-5"></i>
                            <input type="text" x-model="searchQuery" placeholder="Cari NIK, Nama, atau Lokasi..." 
                                   class="w-full pl-12 pr-4 py-3.5 bg-slate-50 border-2 border-slate-100 rounded-2xl outline-blue-600 font-semibold text-sm transition-all focus:bg-white">
                        </div>
                        
                        <div class="flex bg-slate-100 p-1.5 rounded-2xl gap-1">
                            <button @click="currentFilter = 'all'" :class="currentFilter === 'all' ? 'bg-white shadow-sm text-blue-600' : 'text-slate-500'" class="px-5 py-2 rounded-xl text-[10px] font-black uppercase transition-all">SEMUA</button>
                            <button @click="currentFilter = 'open'" :class="currentFilter === 'open' ? 'bg-red-600 text-white shadow-lg' : 'text-slate-500'" class="px-5 py-2 rounded-xl text-[10px] font-black uppercase transition-all">PENDING</button>
                            <button @click="currentFilter = 'close'" :class="currentFilter === 'close' ? 'bg-green-600 text-white shadow-lg' : 'text-slate-500'" class="px-5 py-2 rounded-xl text-[10px] font-black uppercase transition-all">CLOSED</button>
                        </div>
                        
                        <button @click="openModal('nearmiss')" class="bg-[#0f172a] text-white px-8 py-4 rounded-2xl font-black text-xs uppercase tracking-widest hover:bg-blue-600 transition-all shadow-xl shadow-slate-200">
                            + LAPOR ONLINE
                        </button>
                    </div>

                    <div class="bg-white rounded-[2.5rem] border overflow-hidden shadow-sm">
                        <div class="overflow-x-auto">
                            <table class="w-full text-left border-collapse">
                                <thead class="bg-slate-800 text-white font-bold uppercase text-[10px] tracking-widest">
                                    <tr>
                                        <th class="p-6">NIK / Nama</th>
                                        <th class="p-6 text-center">Tanggal</th>
                                        <th class="p-6">Lokasi / Detail</th>
                                        <th class="p-6">Countermeasure</th>
                                        <th class="p-6 text-center">Status</th>
                                        <th class="p-6 text-center">Aksi</th>
                                    </tr>
                                </thead>
                                <tbody class="divide-y text-[11px] font-bold uppercase">
                                    <template x-for="(n, idx) in filteredNearmiss" :key="idx">
                                        <tr class="hover:bg-slate-50 transition-colors">
                                            <td class="p-6">
                                                <div class="text-blue-600 font-black" x-text="n.nik"></div>
                                                <div class="text-slate-400 text-[10px]" x-text="n.nama"></div>
                                            </td>
                                            <td class="p-6 text-center text-slate-500" x-text="n.when"></td>
                                            <td class="p-6 max-w-xs">
                                                <div class="text-slate-800" x-text="n.where"></div>
                                                <div class="text-slate-400 font-medium normal-case line-clamp-1 italic" x-text="n.detail"></div>
                                            </td>
                                            <td class="p-6 max-w-xs truncate text-slate-500 normal-case" x-text="n.measure || '-'"></td>
                                            <td class="p-6 text-center">
                                                <span :class="n.note === 'Close' ? 'bg-green-100 text-green-700' : 'bg-red-100 text-red-700'" 
                                                      class="px-4 py-1.5 rounded-full text-[9px] font-black uppercase inline-block w-24 text-center" 
                                                      x-text="n.note === 'Close' ? 'CLOSED' : 'PENDING'"></span>
                                            </td>
                                            <td class="p-6 text-center">
                                                <div class="flex gap-2 justify-center">
                                                    <button @click="editNearmiss(n)" class="p-2.5 bg-blue-50 text-blue-600 rounded-xl hover:bg-blue-600 hover:text-white transition-all shadow-sm">
                                                        <i data-lucide="edit-3" class="w-4 h-4"></i>
                                                    </button>
                                                    <button @click="deleteData('nearmiss', n)" class="p-2.5 bg-red-50 text-red-600 rounded-xl hover:bg-red-600 hover:text-white transition-all shadow-sm">
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
