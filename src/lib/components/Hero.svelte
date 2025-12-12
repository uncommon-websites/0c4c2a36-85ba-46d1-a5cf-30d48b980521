<script>
  // No imports needed as we use inline SVGs for specific styling control
</script>

<section class="relative flex flex-col items-center justify-start pt-20 pb-32 overflow-hidden bg-black">
  <!-- Content -->
  <div class="z-10 mx-auto max-w-4xl px-4 text-center mb-16">
    <div class="mb-4 inline-block">
      <span class="text-xs font-mono uppercase tracking-widest text-primary-500 border border-primary-500/30 px-3 py-1 rounded-full">
        Launching Q1 2026 • 500+ on Waitlist
      </span>
    </div>
    <h1 class="mb-6 text-5xl md:text-6xl lg:text-7xl font-bold text-white leading-tight">
      Your Personal Analyst.<br/>
      <span class="text-gray-400">Stop Investing Alone.</span>
    </h1>
    <p class="mx-auto mb-10 max-w-2xl text-lg text-gray-400 leading-relaxed">
      Portfolio-specific market intelligence that filters noise and surfaces actionable insights. Built for traders, by traders.
    </p>
    
    <div class="flex justify-center">
        <div class="relative group">
            <button class="relative rounded-md bg-primary-600 px-8 py-3 text-base font-medium text-black hover:bg-primary-500 transition-all font-mono">
                Request Access →
            </button>
            <!-- Decorative corners -->
            <div class="absolute -top-1 -left-1 h-3 w-3 border-t border-l border-primary-500/50"></div>
            <div class="absolute -bottom-1 -right-1 h-3 w-3 border-b border-r border-primary-500/50"></div>
        </div>
    </div>
  </div>

  <!-- Hero Image & Terminal Interface -->
  <div class="relative w-full max-w-7xl mx-auto px-4">
    <div class="relative aspect-[21/9] w-full overflow-hidden rounded-lg shadow-2xl border border-gray-800">
      <img 
        src="/generated/image-multiple-computer-monitors-displaying-st-1765514012507-0.webp" 
        alt="Trading terminal" 
        class="h-full w-full object-cover opacity-40"
      />
      
      <!-- Overlay Terminal Interface -->
      <div class="absolute inset-0 flex items-center justify-center bg-gradient-to-b from-black/60 to-black/80">
        <div class="w-full max-w-2xl rounded-lg bg-gray-950 border border-gray-800 shadow-2xl animate-fade-in-up">
            <!-- Terminal Header -->
            <div class="flex items-center gap-2 px-4 py-2 border-b border-gray-800 bg-gray-900">
              <div class="flex gap-1.5">
                <div class="h-3 w-3 rounded-full bg-red-500/80"></div>
                <div class="h-3 w-3 rounded-full bg-yellow-500/80"></div>
                <div class="h-3 w-3 rounded-full bg-green-500/80"></div>
              </div>
              <span class="text-xs font-mono text-gray-500 ml-2">thesis_terminal</span>
            </div>
            <!-- Terminal Content -->
            <div class="p-4 space-y-2 font-mono text-sm">
              <div class="text-gray-500">$ thesis analyze --portfolio</div>
              <div class="text-primary-400">→ Analyzing your NVDA position...</div>
              <div class="text-gray-400 pl-4">• Unusual volume spike detected (+340%)</div>
              <div class="text-gray-400 pl-4">• IV rank: 87th percentile</div>
              <div class="text-yellow-400 pl-4">⚠ Consider covered call at $145 strike (+2.3% yield)</div>
              <div class="flex items-center gap-2 mt-3">
                <span class="text-gray-500">$</span>
                <span class="text-white">_</span>
                <span class="animate-pulse text-primary-500">▊</span>
              </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
    .animate-fade-in-up {
        animation: fadeInUp 0.8s ease-out forwards;
    }
    @keyframes fadeInUp {
        from { opacity: 0; transform: translateY(20px); }
        to { opacity: 1; transform: translateY(0); }
    }
</style>
