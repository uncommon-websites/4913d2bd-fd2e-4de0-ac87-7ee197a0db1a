<script lang="ts">
  const achievements = [
    "170+ Google Reviews",
    "Top 3 in Brantford",
    "Same-Day Emergency",
    "CDCP Accepted"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-white text-[#1a1a1a]">
  <!-- Background image -->
  <div class="absolute inset-0 z-[-1]">
    <img src="/generated/image-welcoming-dental-reception-area-with-fri-1765492050442-0.webp" alt="Brantford North Dental" class="w-full h-full object-cover opacity-20" />
    <div class="absolute inset-0 bg-gradient-to-b from-white/60 via-white/80 to-white"></div>
  </div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Let our family take care of yours. <span class="text-gray-500">Personalized family dentistry in Brantford with familiar faces, comprehensive treatment options, and a focus on making every patient feel comfortable and cared for.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-70">
    {#each achievements as achievement}
      <div class="h-8 flex items-center justify-center font-medium text-sm">{achievement}</div>
    {/each}
  </div>
</section>
