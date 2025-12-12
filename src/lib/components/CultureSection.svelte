<script lang="ts">
  const cards = [
    {
      title: "We're Not Just Developers...",
      subtitle: "We're Drupal Community Leaders.",
      image: "/generated/image-professional-development-team-collaborat-1765569068786-0.webp"
    },
    {
      title: "We Don't Just Migrate Systems...",
      subtitle: "We Transform Organizations.",
      image: "/generated/image-diverse-software-developers-working-toge-1765569072112-1.webp"
    },
    {
      title: "We Don't Just Follow Agile...",
      subtitle: "We Perfect It For Enterprise.",
      image: "/generated/image-software-engineer-presenting-technical-s-1765569074673-2.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Deep Drupal expertise meets enterprise-grade delivery. We're active contributors to the Drupal community, bringing battle-tested solutions and proven migration strategies to every project.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
