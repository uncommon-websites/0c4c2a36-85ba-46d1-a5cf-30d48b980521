<script>
    const sources = [
        { name: "Bloomberg", icon: "B", color: "bg-orange-600" },
        { name: "MarketWatch", icon: "M", color: "bg-green-700" },
        { name: "Reuters", icon: "R", color: "bg-orange-500" },
        { name: "Unusual Whales", icon: "🐋", color: "bg-blue-600" },
        { name: "Whale Alert", icon: "🚨", color: "bg-red-600" },
        { name: "X / Twitter", icon: "𝕏", color: "bg-black" },
        { name: "Coinbase", icon: "C", color: "bg-blue-500" },
        { name: "Kraken", icon: "K", color: "bg-purple-600" },
        { name: "Fidelity", icon: "F", color: "bg-green-600" },
        { name: "Robinhood", icon: "R", color: "bg-green-500" },
        { name: "Schwab", icon: "S", color: "bg-blue-700" },
        { name: "JPMorgan Chase", icon: "J", color: "bg-blue-800" }
    ];
</script>

<section class="py-24 bg-gray-950">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-16 max-w-2xl">
            <h2 class="text-3xl md:text-4xl font-bold text-white mb-6">Signal Sources & Integrations</h2>
            <p class="text-sm text-gray-400 leading-relaxed">
                Thesis aggregates signals from premium financial data sources and connects directly to your brokerage accounts with read-only access. Bank-level encryption keeps your data secure.
            </p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
            {#each sources as source}
                <div class="flex items-center gap-4 p-4 bg-black border border-gray-800 rounded-lg hover:border-primary-500/50 transition-colors cursor-default">
                    <div class={`h-8 w-8 rounded flex items-center justify-center text-white text-xs font-bold ${source.color}`}>
                        {source.icon}
                    </div>
                    <span class="text-sm font-medium text-gray-300">{source.name}</span>
                </div>
            {/each}
        </div>
    </div>
</section>
