<script lang="ts">
  const projects = [
    {
      client: "Global Healthcare Provider",
      desc: "Migrated legacy systems to Drupal 10, serving 5M+ patients.",
      bg: "bg-[#0a0a1a]",
      img: "/generated/image-modern-healthcare-digital-platform-dashb-1765569231416-0.webp",
      dark: true
    },
    {
      client: "Financial Services Platform",
      desc: "Built enterprise content hub with multi-site architecture.",
      bg: "bg-gray-200",
      img: "/generated/image-financial-services-dashboard-with-data-a-1765569233852-1.webp",
      dark: false
    },
    {
      client: "Manufacturing Enterprise",
      desc: "Integrated Drupal with SAP for seamless data flow.",
      bg: "bg-[#2a2a3e]",
      img: "/generated/image-manufacturing-facility-with-digital-scre-1765569236361-2.webp",
      dark: false
    },
    {
      client: "Education Technology",
      desc: "Scalable learning platform reaching 2M+ students globally.",
      bg: "bg-black",
      img: "/generated/image-students-using-tablets-and-laptops-in-mo-1765569238803-3.webp",
      dark: true
    },
    {
      client: "Retail Transformation",
      desc: "Omnichannel e-commerce platform with headless Drupal.",
      bg: "bg-[#f0f0f0]",
      img: "https://images.unsplash.com/photo-1556742111-a301076d9d18?auto=format&fit=crop&q=80&w=800",
      dark: false,
      full: true // Making full width to align last two items
    },
    {
      client: "Media & Publishing",
      desc: "High-performance content delivery for 10M+ monthly visitors.",
      bg: "bg-[#e8e8e8]",
      img: "https://images.unsplash.com/photo-1504711434969-e33886168f5c?auto=format&fit=crop&q=80&w=800",
      dark: false
    },
    {
      client: "Government Portal",
      desc: "Secure, accessible platform serving citizens nationwide.",
      bg: "bg-[#d0d0e0]",
      img: "https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?auto=format&fit=crop&q=80&w=800",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We deliver enterprise-grade digital platforms</span> powered by Drupal expertise, agile methodology, and proven migration strategies that transform mid-market companies into digital leaders.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
