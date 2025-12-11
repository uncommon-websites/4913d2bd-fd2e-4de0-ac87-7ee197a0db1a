<script lang="ts">
  const services = [
    {
      service: "General Dentistry",
      desc: "Comprehensive dental care for the whole family, from routine checkups to preventive treatments.",
      bg: "bg-gray-50",
      img: "/generated/image-dentist-performing-a-routine-checkup-on--1765492053986-1.webp",
      dark: false
    },
    {
      service: "Cosmetic Dentistry",
      desc: "Transform your smile with professional whitening, veneers, and aesthetic treatments.",
      bg: "bg-gray-50",
      img: "/generated/image-close-up-of-a-patient-smiling-showing-be-1765492057454-2.webp",
      dark: false
    },
    {
      service: "Family Dentistry",
      desc: "Gentle, personalized care for patients of all ages in a comfortable, welcoming environment.",
      bg: "bg-gray-50",
      img: "/generated/image-dentist-examining-a-child-patient-while--1765492059908-3.webp",
      dark: false
    },
    {
      service: "Advanced Technology",
      desc: "High-tech dental equipment and modern techniques for precise, comfortable treatment.",
      bg: "bg-gray-50",
      img: "/generated/image-modern-dental-technology-equipment-in-a--1765492062739-4.webp",
      dark: false
    },
    {
      service: "Emergency Dental Care",
      desc: "Same-day emergency appointments available when you need urgent dental attention.",
      bg: "bg-[oklch(0.262_0.051_172.552)]",
      img: "",
      dark: true,
      full: true
    },
    {
      service: "Canada Dental Care Plan",
      desc: "Proud participants in the CDCP, making quality dental care accessible to more families.",
      bg: "bg-gray-50",
      img: "",
      dark: false
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We offer a wide variety of treatment options</span> to fit each person's unique needs and budgets, ensuring personalized care that helps achieve every smile's potential.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each services as service}
      <div class="group cursor-pointer {service.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${service.bg} mb-4 ${service.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if service.img}
             <img src={service.img} alt={service.service} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for services without images -->
             <div class="w-full h-full flex items-center justify-center p-8">
                <span class={`text-2xl md:text-3xl font-bold text-center ${service.dark ? 'text-white' : 'text-black'}`}>{service.service}</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{service.service}</h3>
        <p class="text-sm text-gray-600">{service.desc}</p>
      </div>
    {/each}
  </div>
</section>
