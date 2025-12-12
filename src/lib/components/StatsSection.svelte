<script lang="ts">
  const stats = [
    {
      label: "200+ Projects",
      desc: "We've successfully delivered over 200 enterprise Drupal projects, from complex migrations to greenfield implementations. Our portfolio spans healthcare, finance, manufacturing, education, and government sectors—each project strengthening our expertise in solving enterprise-scale challenges.",
      img: "https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Drupal Certified",
      desc: "Our team holds multiple Drupal certifications including Acquia Grand Master and Drupal Association memberships. We're active contributors to the Drupal core and maintain several widely-used modules, giving back to the community that powers our success.",
      img: "https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "Global Delivery",
      desc: "With distributed teams across Europe and North America, we provide 24/7 support and seamless collaboration across time zones. Our agile methodology and remote-first culture enable us to deliver enterprise projects efficiently, regardless of location.",
      img: "https://images.unsplash.com/photo-1521737711867-e3b97375f902?auto=format&fit=crop&q=80&w=200"
    },
    {
      label: "$500B Market",
      desc: "We're positioned in the massive IT services transformation market, helping mid-market companies compete with enterprise-grade digital platforms. Our proven migration case studies and Drupal expertise overcome the integration fears that hold CTOs back from digital transformation.",
      img: "/generated/image-professional-cto-or-technology-executive-1765569241344-4.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Numbers that matter. Here's what sets SparkFabrik apart in the enterprise Drupal ecosystem.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
