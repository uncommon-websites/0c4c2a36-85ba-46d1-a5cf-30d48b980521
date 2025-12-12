<script>
  export let active = "Product";
</script>

<header class="sticky top-0 z-50 w-full border-b border-gray-900 bg-black/95 backdrop-blur-sm">
  <div class="mx-auto flex h-16 max-w-7xl items-center justify-between px-4 sm:px-6 lg:px-8">
    <div class="flex items-center gap-8">
      <a href="/" class="flex items-center gap-1">
        <span class="text-xl font-bold tracking-tight font-mono text-white">THESIS</span>
        <span class="text-xl font-bold text-primary-500 animate-pulse">_</span>
      </a>
      
      <nav class="hidden md:flex items-center gap-6">
        {#each ["Product", "Security", "Waitlist"] as item}
          <a href="#{item.toLowerCase()}" class="text-sm font-medium text-gray-400 hover:text-white transition-colors">
            {item}
          </a>
        {/each}
      </nav>
    </div>

    <div class="flex items-center gap-4">
      <a href="#waitlist" class="rounded-md bg-primary-600 px-5 py-2 text-sm font-medium text-black hover:bg-primary-500 transition-colors">
        Request Access
      </a>
    </div>
  </div>
</header>
