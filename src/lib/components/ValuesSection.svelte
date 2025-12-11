<script lang="ts">
  const photos = [
    {
      title: "Modern Technology",
      desc: "We invest in the latest dental technology to provide precise, comfortable, and efficient treatment for all our patients.",
      img: "/generated/image-modern-dental-technology-equipment-in-a--1765492062739-4.webp"
    },
    {
      title: "Comfortable Environment",
      desc: "Our office is designed to reduce anxiety with a welcoming atmosphere, comfortable seating, and a friendly team that remembers you.",
      img: "/generated/image-comfortable-dental-waiting-room-with-nat-1765492071817-7.webp"
    },
    {
      title: "Family-Focused Care",
      desc: "From Tooth Fairy Certificates for kids to gentle care for anxious adults, we make dental visits positive experiences for the whole family.",
      img: "/generated/image-dentist-examining-a-child-patient-while--1765492059908-3.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">We focus on patients, not just procedures.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      In a world of impersonal corporate clinics, we value personal connections and continuity of care. Our practice is built on trust, comfort, and genuine relationships, ensuring every patient feels heard, understood, and cared for—not like just another number.
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
