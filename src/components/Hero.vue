<template>
  <div
    class="relative h-[500px] bg-cover bg-center flex items-center justify-center text-white text-center"
    :style="`background-image: url('${backgroundImage}')`"
  >
    <div
      class="bg-black bg-opacity-60 w-full h-full absolute top-0 left-0"
    ></div>

    <div class="z-10 px-4 max-w-3xl">
      <h1 class="text-4xl font-bold uppercase">
        Compromisso <span class="text-yellow-400">com a qualidade</span>
      </h1>
      <p class="mt-4 text-lg">
        Equipe comprometida com a qualidade e transparência; entre e sinta-se
        bem.
      </p>
      <a
        href="https://www.google.com/search?q=daniel+auto+mec%C3%A2nica+sumare&oq=daniel&gs_lcrp=EgZjaHJvbWUqBggAECMYJzIGCAAQIxgnMgoIARAuGLEDGIAEMgoIAhAuGLEDGIAEMg8IAxAuGBQYhwIYsQMYgAQyDAgEEAAYQxiABBiKBTIGCAUQRRg9MgYIBhBFGD0yBggHEEUYPdIBCDE0NTRqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8&lqi=ChxkYW5pIGF1dG8gbWVjYW5pY2Egc3VtYXJl"
        target="_blank"
        rel="noopener noreferrer"
        class="inline-block mt-6 bg-yellow-400 hover:bg-yellow-500 text-black font-bold py-2 px-6 rounded transition-colors duration-300"
      >
        Ver Avaliações
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeroSection",
  props: {
    backgroundImage: {
      type: String,
      default: "https://path-da-sua-imagem.jpg",
    },
  },
};
</script>
