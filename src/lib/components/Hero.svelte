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

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-[#1a1a2e] via-[#4a4a6a] to-[#fdfbf7] text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#1a1a2e_0%,#3a3a5a_40%,#8a8aa0_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Enterprise-Grade Digital Platforms Built on Drupal Expertise. <span class="text-gray-500">We transform mid-market companies with proven migration strategies, agile methodology, and deep technical knowledge—delivering scalable platforms that drive digital transformation.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 grayscale">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl">{logo}</div>
    {/each}
    <!-- Add more specific logo placeholders if needed -->
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
  </div>
</section>
