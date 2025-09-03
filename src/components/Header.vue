<template>
  <div
    class="bg-black text-white text-sm px-6 py-2 flex justify-between items-center"
  >
    <div class="flex items-center gap-2 text-gray-300">
      <i class="fas fa-clock text-yellow-400"></i>
      <span>Segunda à Sexta: 08:00 - 19:00</span>
    </div>
    <div class="flex gap-4 items-center text-yellow-400">
      <span class="flex items-center gap-1">
        <i class="fas fa-phone"></i> (19) 3832-4765
      </span>

      <div class="flex gap-2"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>
