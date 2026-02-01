<template>
  <header 
    :class="[
      'fixed top-0 w-full z-50 transition-all duration-500 border-b',
      isScrolled ? 'bg-black/90 backdrop-blur-md py-3 border-red-700/50' : 'bg-transparent py-6 border-transparent'
    ]"
  >
    <div class="container mx-auto px-6 flex items-center justify-between">
      
      <NuxtLink to="/" class="flex items-center gap-3 group">
        <img 
          src="/imagenes/inicio/logo_mesa_rock.jpg" 
          alt="Logo" 
          class="w-10 h-10 rounded-full border border-white/20 group-hover:border-red-600 transition-colors"
        />
        <span class="text-white font-black uppercase tracking-tighter text-xl">
          MESA <span class="text-red-700">ROCK</span>
        </span>
      </NuxtLink>

      <nav class="hidden md:flex items-center gap-8">
        <NuxtLink v-for="link in navigation" :key="link.name" :to="link.path" 
          class="text-gray-400 hover:text-white font-bold uppercase text-xs tracking-[0.2em] transition-colors relative group"
        >
          {{ link.name }}
          <span class="absolute -bottom-1 left-0 w-0 h-[2px] bg-red-700 transition-all group-hover:w-full"></span>
        </NuxtLink>
      </nav>

      <div class="flex items-center gap-4">
        <a href="https://www.instagram.com/mesaderockymetalmosquera?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw%3D%3D" target="_blank" rel="noopener noreferrer" class="text-white hover:text-red-600 transition-colors hidden sm:block">
          <span class="text-xs font-mono uppercase">Instagram</span>
        </a>
        <button class="bg-red-700 hover:bg-white hover:text-black text-white px-5 py-2 text-xs font-black uppercase tracking-widest transition-all">
          Unirse
        </button>
      </div>

    </div>
  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const isScrolled = ref(false)

const navigation = [
  { name: 'Inicio', path: '/' },
  { name: 'Nosotros', path: '/nosotros' },
  { name: 'Galería', path: '/galeria' },
  { name: 'Eventos', path: '/eventos' },
]

const handleScroll = () => {
  isScrolled.value = window.scrollY > 50
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<style scoped>
/* Estilo para el link activo de Nuxt */
.router-link-active {
  color: white !important;
}
.router-link-active span {
  width: 100% !important;
}
</style>