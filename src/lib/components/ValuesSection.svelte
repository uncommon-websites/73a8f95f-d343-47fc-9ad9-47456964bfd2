<script lang="ts">
  const photos = [
    {
      title: "Remote-First Culture",
      desc: "Work from anywhere with flexible hours. Our distributed team thrives on asynchronous collaboration and trust.",
      img: "/generated/image-professional-working-remotely-on-laptop--1765569077182-3.webp"
    },
    {
      title: "Community Engagement",
      desc: "Active participation in DrupalCon, local meetups, and open-source contributions. We learn and grow together.",
      img: "/generated/image-tech-professionals-networking-at-develop-1765569079711-4.webp"
    },
    {
      title: "Continuous Learning",
      desc: "Regular training, certifications, and knowledge sharing sessions keep our team at the cutting edge of Drupal.",
      img: "/generated/image-developer-studying-code-on-laptop-screen-1765569082316-5.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We invest in expertise, not just execution.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Our remote-first culture attracts top Drupal talent worldwide. We foster deep technical expertise through continuous learning, community involvement, and collaborative problem-solving—building a team that clients trust for their most critical digital transformations.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
