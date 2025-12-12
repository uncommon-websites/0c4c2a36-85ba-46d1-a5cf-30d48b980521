<script>
    import { Lock, Shield, Eye, FileCheck } from 'lucide-svelte';
</script>

<section class="bg-gray-950 text-white py-24 border-t border-gray-800">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
            <!-- Left Content -->
            <div class="flex flex-col justify-center">
                <div class="flex items-center gap-2 mb-8">
                    <Lock size={16} class="text-primary-500" />
                    <span class="text-xs font-mono uppercase tracking-widest text-gray-400">Security First</span>
                </div>

                <h2 class="text-4xl md:text-5xl font-bold mb-2">Bank-Level Security</h2>
                <h2 class="text-4xl md:text-5xl font-bold text-gray-500 mb-12">For Your Portfolio</h2>

                <div class="space-y-4 mb-12">
                    <div class="flex items-center gap-3">
                        <Lock size={16} class="text-primary-500" />
                        <span class="text-sm font-medium">Read-only broker access (no trade execution)</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <Shield size={16} class="text-primary-500" />
                        <span class="text-sm font-medium">Bank-level encryption standards</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <Eye size={16} class="text-primary-500" />
                        <span class="text-sm font-medium">No data training or sharing</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <FileCheck size={16} class="text-primary-500" />
                        <span class="text-sm font-medium">SOC 2 compliant infrastructure</span>
                    </div>
                </div>

                <a href="#security" class="inline-flex items-center text-sm font-medium text-primary-500 hover:text-primary-400 transition-colors font-mono">
                    Security details <span class="ml-2">→</span>
                </a>
            </div>

            <!-- Right Content: Security Features Grid -->
            <div class="grid grid-cols-2 border border-gray-800 rounded-lg overflow-hidden">
                <!-- Read-Only Access -->
                <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group bg-black hover:bg-gray-900 transition-colors">
                    <div class="h-20 w-20 rounded border-2 border-primary-500/30 flex items-center justify-center mb-4 group-hover:border-primary-500 transition-colors">
                        <Lock size={32} class="text-primary-500" />
                    </div>
                    <span class="text-xs text-gray-400 font-mono text-center">Read-Only<br/>Access</span>
                </div>

                <!-- Encryption -->
                <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group bg-black hover:bg-gray-900 transition-colors">
                    <div class="h-20 w-20 rounded border-2 border-primary-500/30 flex items-center justify-center mb-4 group-hover:border-primary-500 transition-colors">
                        <Shield size={32} class="text-primary-500" />
                    </div>
                    <span class="text-xs text-gray-400 font-mono text-center">Bank-Level<br/>Encryption</span>
                </div>

                <!-- No Training -->
                <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group bg-black hover:bg-gray-900 transition-colors">
                    <div class="h-20 w-20 rounded border-2 border-primary-500/30 flex items-center justify-center mb-4 group-hover:border-primary-500 transition-colors">
                        <Eye size={32} class="text-primary-500" />
                    </div>
                    <span class="text-xs text-gray-400 font-mono text-center">No Data<br/>Training</span>
                </div>

                <!-- SOC 2 -->
                <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group bg-black hover:bg-gray-900 transition-colors">
                    <div class="h-20 w-20 rounded border-2 border-primary-500/30 flex items-center justify-center mb-4 group-hover:border-primary-500 transition-colors">
                        <FileCheck size={32} class="text-primary-500" />
                    </div>
                    <span class="text-xs text-gray-400 font-mono text-center">SOC 2<br/>Compliant</span>
                </div>
            </div>
        </div>
    </div>
</section>
