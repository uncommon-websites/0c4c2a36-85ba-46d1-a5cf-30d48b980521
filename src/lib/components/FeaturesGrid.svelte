<script>
    import { Link, Activity, MessageSquare, TrendingUp, Bell, BarChart3 } from 'lucide-svelte';
</script>

<section class="py-24 bg-black">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-16">
            <h2 class="text-4xl md:text-5xl font-bold text-white leading-tight">
                Built for Traders,<br />
                <span class="text-gray-500">By Traders</span>
            </h2>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Broker Integrations -->
            <div class="bg-gray-950 border border-gray-800 p-8 rounded-lg flex flex-col h-full hover:border-primary-500/50 transition-colors">
                <div class="mb-4">
                    <Link size={24} class="text-primary-500" />
                </div>
                <h3 class="text-lg font-bold text-white mb-4">Broker Integrations</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="grid grid-cols-3 gap-3">
                        {#each ['C', 'K', 'F', 'R', 'S', 'J'] as broker}
                            <div class="h-12 w-12 bg-gray-900 border border-gray-700 rounded flex items-center justify-center text-gray-400 font-mono text-sm hover:border-primary-500/50 hover:text-primary-500 transition-colors">
                                {broker}
                            </div>
                        {/each}
                    </div>
                </div>
                <p class="text-xs text-gray-400 leading-relaxed mt-auto">
                    Direct connections to Coinbase, Kraken, Fidelity, Robinhood, Schwab, and JPMorgan Chase via Snaptrade. Read-only access with bank-level encryption.
                </p>
            </div>

            <!-- Real-Time Monitoring -->
            <div class="bg-gray-950 border border-gray-800 p-8 rounded-lg flex flex-col h-full hover:border-primary-500/50 transition-colors">
                <div class="mb-4">
                    <Activity size={24} class="text-primary-500" />
                </div>
                <h3 class="text-lg font-bold text-white mb-4">Real-Time Monitoring</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-gray-900 border border-gray-800 p-4 rounded w-full max-w-[200px] space-y-3">
                        <div class="flex justify-between items-center">
                            <span class="text-xs text-gray-400 font-mono">NVDA</span>
                            <span class="text-xs text-primary-400 font-mono">+4.2%</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-xs text-gray-400 font-mono">TSLA</span>
                            <span class="text-xs text-red-400 font-mono">-2.1%</span>
                        </div>
                        <div class="flex justify-between items-center">
                            <span class="text-xs text-gray-400 font-mono">AAPL</span>
                            <span class="text-xs text-primary-400 font-mono">+1.8%</span>
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-400 leading-relaxed mt-auto">
                    Live price updates with flash effects on changes. Portfolio monitoring with real-time P&L calculations and buying power tracking.
                </p>
            </div>

            <!-- AI Copilot -->
            <div class="bg-gray-950 border border-gray-800 p-8 rounded-lg flex flex-col h-full hover:border-primary-500/50 transition-colors">
                <div class="mb-4">
                    <MessageSquare size={24} class="text-primary-500" />
                </div>
                <h3 class="text-lg font-bold text-white mb-4">AI Copilot</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-gray-900 border border-gray-800 p-4 rounded w-full max-w-[200px] space-y-2">
                        <div class="text-[10px] text-gray-500 font-mono">$ thesis analyze</div>
                        <div class="text-[9px] text-primary-400 leading-relaxed">
                            Your NVDA position is up 4.2%. IV rank at 67th percentile suggests covered call opportunity...
                        </div>
                        <div class="flex items-center gap-1 mt-2">
                            <span class="text-[10px] text-gray-500 font-mono">$</span>
                            <span class="animate-pulse text-primary-500">▊</span>
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-400 leading-relaxed mt-auto">
                    Natural language interface for portfolio queries. Ask about positions, get strategy recommendations, analyze options Greeks, and receive actionable insights.
                </p>
            </div>

            <!-- Options Analysis -->
            <div class="bg-gray-950 border border-gray-800 p-8 rounded-lg flex flex-col h-full hover:border-primary-500/50 transition-colors">
                <div class="mb-4">
                    <TrendingUp size={24} class="text-primary-500" />
                </div>
                <h3 class="text-lg font-bold text-white mb-4">Options Intelligence</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-gray-900 border border-gray-800 p-4 rounded w-full max-w-[200px] space-y-2">
                        <div class="text-[10px] text-gray-400">AAPL $145 Call</div>
                        <div class="space-y-1 text-[9px]">
                            <div class="flex justify-between">
                                <span class="text-gray-500">IV Rank:</span>
                                <span class="text-primary-400">67%</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-500">Theta:</span>
                                <span class="text-gray-400">-$0.12</span>
                            </div>
                            <div class="flex justify-between">
                                <span class="text-gray-500">Delta:</span>
                                <span class="text-gray-400">0.68</span>
                            </div>
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-400 leading-relaxed mt-auto">
                    Track IV rank and percentile, expected moves, Greeks analysis, strike optimization, and theta decay vs gamma risk balancing.
                </p>
            </div>

            <!-- Proactive Alerts -->
            <div class="bg-gray-950 border border-gray-800 p-8 rounded-lg flex flex-col h-full hover:border-primary-500/50 transition-colors">
                <div class="mb-4">
                    <Bell size={24} class="text-primary-500" />
                </div>
                <h3 class="text-lg font-bold text-white mb-4">Proactive Alerts</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-gray-900 border border-yellow-500/20 p-4 rounded w-full max-w-[200px] space-y-2">
                        <div class="flex items-center gap-2">
                            <span class="text-yellow-400 text-xs">⚠</span>
                            <span class="text-[10px] text-yellow-400 font-mono">ALERT</span>
                        </div>
                        <div class="text-[9px] text-gray-300">
                            TSLA calls expire in 3 days. Consider rolling or closing position.
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-400 leading-relaxed mt-auto">
                    Unusual volatility detection, expiring options reminders, cost basis alerts, and opportunity identification that doesn't wait to be asked.
                </p>
            </div>

            <!-- Signal Feed -->
            <div class="bg-gray-950 border border-gray-800 p-8 rounded-lg flex flex-col h-full hover:border-primary-500/50 transition-colors">
                <div class="mb-4">
                    <BarChart3 size={24} class="text-primary-500" />
                </div>
                <h3 class="text-lg font-bold text-white mb-4">Signal Feed</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-gray-900 border border-gray-800 p-4 rounded w-full max-w-[200px] space-y-2">
                        <div class="flex items-center gap-2 text-[9px]">
                            <div class="h-1.5 w-1.5 rounded-full bg-primary-500"></div>
                            <span class="text-gray-400">Bloomberg: NVDA earnings beat</span>
                        </div>
                        <div class="flex items-center gap-2 text-[9px]">
                            <div class="h-1.5 w-1.5 rounded-full bg-primary-500"></div>
                            <span class="text-gray-400">Unusual Whales: $2M call sweep</span>
                        </div>
                        <div class="flex items-center gap-2 text-[9px]">
                            <div class="h-1.5 w-1.5 rounded-full bg-primary-500"></div>
                            <span class="text-gray-400">Reuters: Fed rate decision</span>
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-400 leading-relaxed mt-auto">
                    Aggregated signals from Bloomberg, MarketWatch, Reuters, Unusual Whales, Whale Alert, and social media filtered for your portfolio.
                </p>
            </div>
        </div>
    </div>
</section>
