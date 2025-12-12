<script lang="ts">
  // Enterprise client logos
  const logos = [
    "Accenture",
    "Deloitte",
    "IBM",
    "SAP",
    "Oracle"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 text-white overflow-hidden">
  <!-- Background Image -->
  <div class="absolute inset-0 z-[-2]">
    <img 
      src="/generated/image-modern-enterprise-office-with-developers-1765573656198-0.webp" 
      alt="Enterprise digital workspace"
      class="w-full h-full object-cover"
    />
  </div>
  
  <!-- Dark overlay for text readability -->
  <div class="absolute inset-0 z-[-1] bg-gradient-to-b from-gray-900/90 via-gray-900/80 to-gray-900/95"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight text-white">
      Enterprise-Grade Digital Platforms Built on Drupal Expertise. <span class="text-gray-300">We transform mid-market companies with proven migration strategies, agile methodology, and deep technical knowledge—delivering scalable platforms that drive digital transformation.</span>
    </h1>
  </div>

  <div class="border-t border-white/30 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-70">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl text-white">{logo}</div>
    {/each}
    <!-- Add more specific logo placeholders if needed -->
    <div class="h-8 w-20 bg-white/20 rounded"></div>
    <div class="h-8 w-20 bg-white/20 rounded"></div>
    <div class="h-8 w-20 bg-white/20 rounded"></div>
  </div>
</section>
