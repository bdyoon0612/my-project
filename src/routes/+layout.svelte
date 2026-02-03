<script>
    import '../app.css';
</script>

<div class="h-12 w-full"></div>

<nav class="px-6 py-4 flex items-center justify-between sticky top-0 z-50 bg-background-light/80 dark:bg-background-dark/80 backdrop-blur-md">
    <div class="flex items-center gap-1">
        <span class="text-2xl font-black tracking-tight text-slate-900 dark:text-white">Tennis<span class="text-primary">Pro</span></span>
    </div>
    <div class="flex items-center gap-4">
        <button class="p-2 rounded-full bg-slate-100 dark:bg-slate-800">
            <span class="material-icons text-xl">search</span>
        </button>
        <button class="p-2 rounded-full bg-slate-100 dark:bg-slate-800">
            <span class="material-icons text-xl">notifications_none</span>
        </button>
    </div>
</nav>

<slot />

<div class="fixed bottom-0 left-0 right-0 bg-white/90 dark:bg-slate-900/90 backdrop-blur-lg border-t border-slate-200 dark:border-slate-800 px-8 py-3 flex justify-between items-center z-50">
    <div class="flex flex-col items-center gap-1 text-primary">
        <span class="material-icons">home</span>
        <span class="text-[10px] font-bold">홈</span>
    </div>
    <div class="flex flex-col items-center gap-1 text-slate-400 dark:text-slate-500">
        <span class="material-icons">event_available</span>
        <span class="text-[10px] font-bold">예약</span>
    </div>
    <div class="relative -top-8">
        <button class="w-14 h-14 bg-primary rounded-full shadow-lg shadow-primary/40 flex items-center justify-center text-white active:scale-90 transition-transform">
            <span class="material-icons text-3xl">add</span>
        </button>
    </div>
    <div class="flex flex-col items-center gap-1 text-slate-400 dark:text-slate-500">
        <span class="material-icons">school</span>
        <span class="text-[10px] font-bold">레슨</span>
    </div>
    <div class="flex flex-col items-center gap-1 text-slate-400 dark:text-slate-500">
        <span class="material-icons">emoji_events</span>
        <span class="text-[10px] font-bold">대회</span>
    </div>
</div>
<div class="fixed bottom-1 left-1/2 -translate-x-1/2 w-32 h-1.5 bg-slate-300 dark:bg-slate-700 rounded-full z-[60]"></div>
