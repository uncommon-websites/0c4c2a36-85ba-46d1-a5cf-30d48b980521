<script>
    import { ArrowLeft, ArrowRight } from 'lucide-svelte';
</script>

<section class="bg-gray-950 py-24 overflow-hidden border-t border-gray-800">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <!-- Navigation Buttons -->
        <div class="flex justify-end gap-2 mb-8">
            <button class="h-10 w-10 rounded border border-gray-700 flex items-center justify-center bg-black hover:bg-gray-900 transition-colors text-gray-400 hover:text-primary-500">
                <ArrowLeft size={16} />
            </button>
            <button class="h-10 w-10 rounded border border-gray-700 flex items-center justify-center bg-black hover:bg-gray-900 transition-colors text-gray-400 hover:text-primary-500">
                <ArrowRight size={16} />
            </button>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
            <!-- Quote Content -->
            <div class="pr-8">
                <div class="mb-8">
                    <span class="text-sm font-bold tracking-widest uppercase text-primary-500">Waitlist User • $320K Portfolio</span>
                </div>
                <blockquote class="text-2xl md:text-3xl font-light text-white leading-relaxed mb-12">
                    "I've been trading actively for 8 years and the amount of noise I have to filter through every day is exhausting. Thesis understanding my actual positions and alerting me to what matters—that's the game changer I've been waiting for."
                </blockquote>
                <div>
                    <div class="font-medium text-white">Michael R.</div>
                    <div class="text-[10px] uppercase tracking-widest text-gray-500 mt-1 font-mono">Active Options Trader • Joined Waitlist Nov 2024</div>
                </div>
            </div>

            <!-- Image -->
            <div class="relative h-[600px] w-full overflow-hidden rounded-lg border border-gray-800">
                <img 
                    src="/generated/image-confident-trader-in-their-30s-looking-at-1765514018020-2.webp" 
                    alt="Active trader" 
                    class="absolute inset-0 h-full w-full object-cover opacity-60"
                />
                <!-- Terminal overlay effect -->
                <div class="absolute inset-0 bg-gradient-to-t from-gray-950 via-transparent to-transparent"></div>
            </div>
        </div>
    </div>
</section>
