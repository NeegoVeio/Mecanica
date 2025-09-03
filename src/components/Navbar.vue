<template>
  <nav class="bg-black text-white px-6 py-4">
    <div class="flex items-center justify-between">
      <img
        src="@/assets/logomec2.png"
        alt="Logo"
        class="h-20 w-auto object-contain"
      />

      <ul class="flex gap-6 text-sm font-semibold text-yellow-400">
        <li><a href="#sobre-nos">SOBRE NÓS</a></li>
        <li><a href="#servicos">SERVIÇOS</a></li>
        <li>
          <a
            href="https://www.google.com/maps/place/Auto+Mecanica+Daniel/@-22.8063596,-47.2044451,17z/data=!3m1!4b1!4m6!3m5!1s0x94c8bf6b41c4c6d3:0x43ffe7d19ff3456d!8m2!3d-22.8063596!4d-47.2018702!16s%2Fg%2F11khm021y1?entry=ttu&g_ep=EgoyMDI1MDgyNS4wIKXMDSoASAFQAw%3D%3D"
            target="_blank"
            >LOCALIZAÇÃO</a
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "MainNavbar",
};
</script>
