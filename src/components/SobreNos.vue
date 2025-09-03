<template>
  <section id="sobre-nos" class="max-w-6xl mx-auto p-6">
    <h2 class="text-3xl font-bold mb-6 text-yellow-400">Sobre Nós</h2>
    <div class="flex flex-col md:flex-row gap-8">
      <div class="md:w-1/2 text-gray-800">
        <p class="mb-4">
          Fundada há mais de 20 anos, a Auto Mecânica Daniel é referência em
          qualidade e confiança em Sumaré. Nossa equipe é formada por
          profissionais qualificados que garantem o melhor serviço para o seu
          veículo.
        </p>
        <p>
          Prezamos pela transparência e pelo atendimento personalizado, buscando
          sempre a satisfação dos nossos clientes.
        </p>
      </div>

      <div class="md:w-1/2 relative">
        <img
          :src="images[currentIndex]"
          alt="Sobre Nós"
          class="rounded-lg w-full h-64 object-cover"
        />

        <button
          @click="prevSlide"
          class="absolute top-1/2 left-2 transform -translate-y-1/2 bg-yellow-400 text-black p-2 rounded-full hover:bg-yellow-500"
        >
          ‹
        </button>
        <button
          @click="nextSlide"
          class="absolute top-1/2 right-2 transform -translate-y-1/2 bg-yellow-400 text-black p-2 rounded-full hover:bg-yellow-500"
        >
          ›
        </button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SobreNos",
  data() {
    return {
      images: [
        "https://images.unsplash.com/photo-1503376780353-7e6692767b70?auto=format&fit=crop&w=800&q=80",
        "https://images.unsplash.com/photo-1549924231-f129b911e442?auto=format&fit=crop&w=800&q=80",
        "https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80",
      ],
      currentIndex: 0,
      intervalId: null,
    };
  },
  mounted() {
    this.startAutoSlide();
  },
  beforeUnmount() {
    clearInterval(this.intervalId);
  },
  methods: {
    nextSlide() {
      this.currentIndex = (this.currentIndex + 1) % this.images.length;
    },
    prevSlide() {
      this.currentIndex =
        (this.currentIndex - 1 + this.images.length) % this.images.length;
    },
    startAutoSlide() {
      this.intervalId = setInterval(this.nextSlide, 4000);
    },
  },
};
</script>
