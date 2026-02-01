<template>
  <section class="bg-black py-24 overflow-hidden">
    <div class="container mx-auto px-6">
      <div class="mb-16 text-center md:text-left flex flex-col md:flex-row md:items-end justify-between gap-6">
        <div>
          <span class="text-red-700 font-mono tracking-[0.5em] uppercase text-sm block mb-2">Registro Visual</span>
          <h2 class="text-6xl md:text-8xl font-black text-white uppercase tracking-tighter leading-none">
            EL <span class="italic text-transparent text-stroke-white">PIT</span> <br/> EN LENTES
          </h2>
        </div>
        <p class="text-gray-500 max-w-sm font-light text-lg">
          Capturando la energía, el sudor y la pasión de cada encuentro metalero en Mosquera.
        </p>
      </div>

      <div class="grid grid-cols-2 md:grid-cols-4 gap-4 auto-rows-[200px]">
        
        <div class="relative group overflow-hidden md:col-span-2 md:row-span-2">
          <img src="https://images.unsplash.com/photo-1516450360452-9312f5e86fc7?q=80&w=2070" 
               class="w-full h-full object-cover grayscale group-hover:grayscale-0 group-hover:scale-110 transition-all duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-red-900/80 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
            <span class="text-white font-bold uppercase italic">Concierto Lanzamiento 2024</span>
          </div>
        </div>

        <div class="relative group overflow-hidden md:row-span-2">
          <img src="https://images.unsplash.com/photo-1459749411177-042180ce673c?q=80&w=2070" 
               class="w-full h-full object-cover grayscale group-hover:grayscale-0 group-hover:scale-110 transition-all duration-700" />
        </div>

        <div class="relative group overflow-hidden">
          <img src="https://images.unsplash.com/photo-1514525253361-bee8718a74a2?q=80&w=1964" 
               class="w-full h-full object-cover grayscale group-hover:grayscale-0 group-hover:scale-110 transition-all duration-700" />
        </div>

        <div class="relative group overflow-hidden">
          <img src="https://images.unsplash.com/photo-1524715858092-23e845c5773c?q=80&w=2070" 
               class="w-full h-full object-cover grayscale group-hover:grayscale-0 group-hover:scale-110 transition-all duration-700" />
        </div>

        <div class="relative group overflow-hidden md:col-span-2">
          <img src="https://images.unsplash.com/photo-1470229722913-7c0e2dbbafd3?q=80&w=2070" 
               class="w-full h-full object-cover grayscale group-hover:grayscale-0 group-hover:scale-110 transition-all duration-700" />
        </div>
      </div>

      <div class="mt-16 text-center">
        <button class="group relative px-12 py-4 border-2 border-white text-white font-black uppercase tracking-widest overflow-hidden transition-all">
          <span class="absolute inset-0 w-0 bg-white transition-all duration-300 group-hover:w-full"></span>
          <span class="relative group-hover:text-black transition-colors">Ver Galería Completa</span>
        </button>
      </div>
    </div>
  </section>
</template>

<style scoped>
.text-stroke-white {
  -webkit-text-stroke: 1px white;
}
</style>