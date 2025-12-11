<script lang="ts">
  const stats = [
    {
      label: "170+ Reviews",
      desc: "With over 170 Google reviews and an 'Excellent' rating, our patients consistently praise our personalized care, gentle approach, and ability to make even the most anxious patients feel comfortable. Our reputation is built on trust and word-of-mouth referrals from satisfied families.",
      img: "/generated/image-happy-middle-aged-patient-leaving-dental-1765492075074-8.webp"
    },
    {
      label: "Top 3 in Brantford",
      desc: "Named one of the top three dental offices in Brantford by ThreeBestRated.ca for three consecutive years (2019-2021). This recognition reflects our commitment to quality care, modern technology, and exceptional patient service.",
      img: "/generated/image-happy-middle-aged-patient-leaving-dental-1765492075074-8.webp"
    },
    {
      label: "CDCP Participant",
      desc: "We're proud participants in the Canada Dental Care Plan (CDCP), making quality dental care more accessible to families across Brantford. We believe everyone deserves excellent dental care, regardless of their financial situation.",
      img: "/generated/image-happy-middle-aged-patient-leaving-dental-1765492075074-8.webp"
    },
    {
      label: "Same-Day Emergency",
      desc: "Dental emergencies don't wait, and neither do we. We offer same-day emergency appointments and work hard to fit you in quickly when you're experiencing tooth pain or urgent dental issues. Your comfort and health are our priority.",
      img: "/generated/image-happy-middle-aged-patient-leaving-dental-1765492075074-8.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Curious about what sets us apart? Here's a snapshot of our practice, our achievements, and the commitments we're proud of.
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
