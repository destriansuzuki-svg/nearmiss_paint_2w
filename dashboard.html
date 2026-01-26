<?php 
// Di sini nanti bisa ditambah pengecekan session login jika diperlukan
?>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard - Painting 2W</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script defer src="https://unpkg.com/alpinejs@3.x.x/dist/cdn.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>[x-cloak] { display: none !important; } body { font-family: 'Plus Jakarta Sans', sans-serif; }</style>
</head>
<body class="bg-slate-50" x-data="appData()" x-init="initApp('dashboard')">

    <div class="flex h-screen w-full overflow-hidden">
        <?php include 'layout_sidebar.php'; ?>

        <div class="flex-1 flex flex-col min-w-0 overflow-hidden">
            <header class="bg-white border-b px-8 py-4 flex justify-between items-center z-40">
                <h2 class="text-xl font-extrabold text-slate-800 uppercase">Dashboard Statistik</h2>
                <div class="flex items-center gap-4">
                    <button @click="syncAll()" class="bg-blue-50 text-blue-600 px-4 py-2 rounded-xl font-bold text-xs" 
                            x-text="isSyncing ? 'SINKRON...' : 'REFRESH DATA'"></button>
                </div>
            </header>

            <main class="flex-1 overflow-y-auto p-6 lg:p-10 space-y-8">
                <div class="bg-white p-4 rounded-2xl border flex items-center gap-4 shadow-sm">
                    <span class="text-[10px] font-black text-slate-400 uppercase">Filter Range:</span>
                    <input type="date" x-model="startDate" @change="updateDashboard()" class="p-2 border rounded-xl text-xs font-bold outline-blue-600">
                    <span class="text-slate-300">-</span>
                    <input type="date" x-model="endDate" @change="updateDashboard()" class="p-2 border rounded-xl text-xs font-bold outline-blue-600">
                </div>

                <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                    <div class="bg-white p-6 rounded-[2rem] border-2 border-blue-50 text-center shadow-sm">
                        <p class="text-[10px] font-black text-blue-500 uppercase">Total Nearmiss</p>
                        <h4 class="text-4xl font-black text-blue-600 mt-2" x-text="filteredNearmissDashboard.length"></h4>
                    </div>
                    <div class="bg-white p-6 rounded-[2rem] border-2 border-red-50 text-center shadow-sm">
                        <p class="text-[10px] font-black text-red-500 uppercase">Pending (Open)</p>
                        <h4 class="text-4xl font-black text-red-600 mt-2" x-text="stats.open"></h4>
                    </div>
                    <div class="bg-white p-6 rounded-[2rem] border-2 border-green-50 text-center shadow-sm">
                        <p class="text-[10px] font-black text-green-500 uppercase">Closed</p>
                        <h4 class="text-4xl font-black text-green-600 mt-2" x-text="stats.close"></h4>
                    </div>
                    <div class="bg-white p-6 rounded-[2rem] border-2 border-slate-50 text-center shadow-sm">
                        <p class="text-[10px] font-black text-slate-400 uppercase">Karyawan Aktif</p>
                        <h4 class="text-4xl font-black text-slate-800 mt-2" x-text="karyawan.length"></h4>
                    </div>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
                    <div class="lg:col-span-2 bg-white p-8 rounded-[2.5rem] border shadow-sm h-80">
                        <h4 class="text-[10px] font-black text-slate-400 uppercase mb-4 tracking-widest">Temuan Per Bulan Fiskal (Apr-Mar)</h4>
                        <div class="h-64"><canvas id="barChart"></canvas></div>
                    </div>
                    <div class="bg-white p-8 rounded-[2.5rem] border shadow-sm h-80 flex flex-col">
                        <h4 class="text-[10px] font-black text-slate-400 uppercase mb-4 text-center tracking-widest">Persentase Status</h4>
                        <div class="flex-1"><canvas id="pieChart"></canvas></div>
                    </div>
                </div>

                <div class="bg-white p-8 rounded-[2.5rem] border shadow-sm">
                    <h4 class="font-black text-slate-800 mb-6 uppercase text-xs tracking-widest">Log Temuan Terbaru</h4>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <template x-for="log in nearmiss.slice(0,6)" :key="log.when + log.nik">
                            <div class="flex items-center gap-4 p-5 bg-slate-50 rounded-2xl border-l-4 border-blue-500 transition-hover hover:shadow-md">
                                <div class="flex-1">
                                    <p class="text-[11px] font-bold text-slate-700 leading-relaxed">
                                        <span class="text-blue-600 font-black" x-text="log.nama"></span> mendeteksi bahaya di <span class="font-black" x-text="log.where"></span>
                                    </p>
                                    <p class="text-[9px] text-slate-400 font-bold mt-1 uppercase" x-text="log.when"></p>
                                </div>
                                <span :class="log.note === 'Close' ? 'bg-green-100 text-green-600' : 'bg-red-100 text-red-600'" 
                                      class="px-3 py-1 rounded-lg text-[9px] font-black uppercase" x-text="log.note"></span>
                            </div>
                        </template>
                    </div>
                </div>
            </main>
        </div>
    </div>

    <?php include 'layout_footer_js.php'; ?>
</body>
</html>
