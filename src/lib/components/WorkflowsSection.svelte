<script>
    import { Check, ArrowRight, Sun, AlertTriangle, TrendingUp } from 'lucide-svelte';
</script>

<section class="py-24 bg-black">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-16">
            <h2 class="text-4xl md:text-5xl font-bold text-white leading-tight">
                Proactive Intelligence<br />
                <span class="text-gray-500">That Doesn't Wait To Be Asked</span>
            </h2>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Card 1: Morning Briefing -->
            <div class="group">
                <div class="mb-6 bg-gray-950 border border-gray-800 rounded-lg p-6 aspect-[4/3] relative overflow-hidden flex flex-col">
                    <!-- Mock Interface -->
                    <div class="bg-gray-900 border border-primary-500/20 rounded-lg p-4 shadow-lg w-full max-w-[90%] mx-auto mt-auto mb-4 transform translate-y-2 transition-transform group-hover:translate-y-0">
                        <div class="flex items-center gap-2 mb-3 border-b border-gray-800 pb-2">
                            <Sun size={12} class="text-primary-500" />
                            <span class="text-[10px] font-mono text-gray-400">Morning Briefing • 8:30 AM</span>
                        </div>
                        <div class="space-y-2 text-xs">
                            <div class="text-primary-400">Portfolio: +2.3% ($4,821)</div>
                            <div class="text-gray-400">• NVDA up 4.2% on earnings beat</div>
                            <div class="text-gray-400">• TSLA calls expire Friday</div>
                            <div class="text-yellow-400">⚠ SPY correlation risk: 0.87</div>
                        </div>
                    </div>
                </div>
                <h3 class="text-xl font-bold text-white mb-3">Morning Briefing</h3>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Start your day with portfolio performance, what's moving and why, attention-needed items like expiring options, and opportunity identification for covered calls or rolling strategies.
                </p>
            </div>

            <!-- Card 2: Risk Alerts -->
            <div class="group">
                <div class="mb-6 bg-gray-950 border border-gray-800 rounded-lg p-6 aspect-[4/3] relative overflow-hidden flex flex-col">
                     <!-- Mock Interface -->
                     <div class="bg-gray-900 border border-red-500/20 rounded-lg p-4 shadow-lg w-full max-w-[90%] mx-auto mt-auto mb-4 transform translate-y-2 transition-transform group-hover:translate-y-0">
                        <div class="flex items-center gap-2 mb-3">
                            <AlertTriangle size={12} class="text-red-500" />
                            <span class="text-[10px] font-mono text-red-400">RISK ALERT</span>
                        </div>
                        <div class="space-y-2 text-xs">
                            <div class="text-white">TSLA Position Alert</div>
                            <div class="text-gray-400">• Unusual volatility: +340%</div>
                            <div class="text-gray-400">• Total exposure: $28,800</div>
                            <div class="text-yellow-400">→ Suggested hedge: $140 put</div>
                        </div>
                    </div>
                </div>
                <h3 class="text-xl font-bold text-white mb-3">Risk Alert System</h3>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Get proactive alerts on unusual volatility, exposure analysis across direct and correlated positions, total at-risk calculations, and suggested hedge recommendations with specific strikes.
                </p>
            </div>

            <!-- Card 3: Options Analysis -->
            <div class="group">
                <div class="mb-6 bg-gray-950 border border-gray-800 rounded-lg p-6 aspect-[4/3] relative overflow-hidden flex flex-col">
                     <!-- Mock Interface -->
                     <div class="bg-gray-900 border border-primary-500/20 rounded-lg p-4 shadow-lg w-full max-w-[90%] mx-auto mt-auto mb-4 transform translate-y-2 transition-transform group-hover:translate-y-0">
                        <div class="flex items-center gap-2 mb-3">
                            <TrendingUp size={12} class="text-primary-500" />
                            <span class="text-[10px] font-mono text-gray-400">Options Analysis</span>
                        </div>
                        <div class="space-y-2 text-xs">
                            <div class="text-white">AAPL $145 Call • Exp: 2/21</div>
                            <div class="flex justify-between text-gray-400">
                                <span>IV Rank:</span>
                                <span class="text-primary-400">67th percentile</span>
                            </div>
                            <div class="flex justify-between text-gray-400">
                                <span>Theta:</span>
                                <span>-$0.12/day</span>
                            </div>
                            <div class="text-primary-400 mt-2">→ Roll to $150 for +$0.45 credit</div>
                        </div>
                    </div>
                </div>
                <h3 class="text-xl font-bold text-white mb-3">Options Intelligence</h3>
                <p class="text-sm text-gray-400 leading-relaxed">
                    Track IV rank and percentile, expected move calculations, Greeks analysis, strike optimization for specific targets, and theta decay vs gamma risk balancing with buying power checks.
                </p>
            </div>
        </div>
    </div>
</section>
