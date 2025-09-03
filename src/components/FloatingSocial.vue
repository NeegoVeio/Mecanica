<template>
  <div
    class="fixed bottom-6 right-6 z-50"
    @mouseenter="showMenu = true"
    @mouseleave="showMenu = false"
  >
    <!-- Botão principal (WhatsApp ícone) -->
    <div
      class="bg-green-500 w-14 h-14 rounded-full flex items-center justify-center shadow-lg cursor-pointer transition duration-300 ease-in-out hover:scale-110"
    >
      <i class="fab fa-whatsapp text-white text-2xl"></i>
    </div>

    <!-- Menu flutuante -->
    <transition name="fade">
      <div
        v-if="showMenu"
        class="absolute bottom-16 right-0 flex flex-col gap-3 bg-white rounded-lg p-3 shadow-xl"
      >
        <a
          href="https://wa.me/5519992670097"
          target="_blank"
          class="flex items-center gap-2 text-green-600 hover:underline"
        >
          <i class="fab fa-whatsapp text-xl"></i> WhatsApp
        </a>
        <a
          href="https://www.facebook.com/ameliacar/?locale=pt_BR"
          target="_blank"
          class="flex items-center gap-2 text-pink-500 hover:underline"
        >
          <i class="fab fa-instagram text-xl"></i> Instagram
        </a>
        <a
          href="https://www.facebook.com/ameliacar/?locale=pt_BR"
          target="_blank"
          class="flex items-center gap-2 text-blue-600 hover:underline"
        >
          <i class="fab fa-facebook text-xl"></i> Facebook
        </a>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: "FloatingSocial",
  data() {
    return {
      showMenu: false,
    };
  },
};
</script>

<style>
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease;
}
.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
