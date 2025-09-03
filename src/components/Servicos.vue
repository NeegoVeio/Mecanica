<template>
  <section id="servicos" class="py-16 bg-gray-100 text-black">
    <div class="max-w-6xl mx-auto px-4">
      <h2 class="text-3xl font-bold text-center mb-10">Nossos Serviços</h2>

      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
        <div class="bg-white shadow-md p-6 rounded text-center">
          <i class="fas fa-tools text-4xl text-yellow-500 mb-4"></i>
          <h3 class="text-xl font-semibold mb-2">Manutenção Preventiva</h3>
          <p>
            Evite imprevistos com revisões periódicas e cuidados essenciais.
          </p>
        </div>

        <div class="bg-white shadow-md p-6 rounded text-center">
          <i class="fas fa-car-crash text-4xl text-yellow-500 mb-4"></i>
          <h3 class="text-xl font-semibold mb-2">Suspensão & Freios</h3>
          <p>
            Verificação completa do sistema de freios e componentes da
            suspensão.
          </p>
        </div>

        <div class="bg-white shadow-md p-6 rounded text-center">
          <i class="fas fa-oil-can text-4xl text-yellow-500 mb-4"></i>
          <h3 class="text-xl font-semibold mb-2">Troca de Óleo</h3>
          <p>Serviço rápido com óleo e filtro de qualidade.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ServicosSection",
};
</script>
