<script>
    import { TrendingUp, Shield, Zap, Target } from 'lucide-svelte';
</script>

<section class="py-24 bg-gray-950">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-20">
            <h2 class="text-4xl md:text-5xl font-bold text-white leading-tight max-w-4xl">
                Context-aware intelligence that knows your <span class="text-primary-500">actual portfolio positions</span>
            </h2>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
            <!-- Left: Image/Interface -->
            <div class="relative">
                <div class="relative rounded-lg overflow-hidden shadow-2xl bg-black border border-gray-800 aspect-[4/3]">
                    <img 
                        src="/generated/image-close-up-of-hands-typing-on-a-keyboard-w-1765514015027-1.webp" 
                        alt="Trading screens" 
                        class="absolute inset-0 w-full h-full object-cover opacity-20"
                    />
                    
                    <!-- Floating Alert Card -->
                    <div class="absolute inset-0 flex items-center justify-center p-8">
                        <div class="bg-gray-900 border border-primary-500/30 rounded-lg shadow-xl w-full max-w-md p-6">
                            <div class="flex items-center gap-3 mb-4">
                                <div class="h-8 w-8 bg-primary-600 rounded flex items-center justify-center text-black">
                                    <Zap size={16} />
                                </div>
                                <span class="font-medium text-white font-mono text-sm">RISK ALERT</span>
                            </div>
                            <div class="space-y-3 text-sm">
                                <div class="text-gray-300">Your TSLA position (240 shares)</div>
                                <div class="text-yellow-400">⚠ Unusual volatility spike detected</div>
                                <div class="text-gray-400 text-xs">IV rank: 92nd percentile • Consider hedging</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Right: Features List -->
            <div class="space-y-12">
                <h3 class="text-2xl font-bold text-white">
                    Intelligence That Understands<br/> Your Portfolio, Not Just Markets
                </h3>

                <div class="space-y-8">
                    {#each [
                        { id: '01', title: 'Portfolio-specific insights', icon: Target },
                        { id: '02', title: 'Proactive risk alerts', icon: Shield },
                        { id: '03', title: 'Options-savvy analysis', icon: TrendingUp },
                        { id: '04', title: 'Read-only broker connections', icon: Zap }
                    ] as feature}
                        <div class="flex items-start gap-4 group cursor-pointer">
                            <div class="flex-shrink-0 relative">
                                <div class="h-10 w-10 rounded border border-gray-700 flex items-center justify-center text-xs font-mono text-gray-500 group-hover:border-primary-500 group-hover:text-primary-500 transition-colors bg-gray-900 z-10 relative">
                                    {feature.id}
                                </div>
                                {#if feature.id !== '04'}
                                    <div class="absolute top-10 left-1/2 -translate-x-1/2 w-px h-8 bg-gray-800 -z-0"></div>
                                {/if}
                            </div>
                            <div class="pt-2">
                                <h4 class="text-lg text-gray-400 group-hover:text-white transition-colors">
                                    {feature.title}
                                </h4>
                            </div>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>
</section>
