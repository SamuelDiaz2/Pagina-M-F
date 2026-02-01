<template>
  <main class="min-h-screen bg-[#050505] text-white pt-24 pb-20">
    <div class="container mx-auto px-6">
      
      <header class="mb-20 text-center">
        <span class="text-red-700 font-mono tracking-[0.5em] uppercase text-sm">Detrás del Ruido</span>
        <h1 class="text-7xl md:text-9xl font-black uppercase tracking-tighter leading-none mt-4">
          NUESTRO <br/> <span class="text-transparent text-stroke-white italic">EQUIPO</span>
        </h1>
        <p class="text-gray-400 mt-8 max-w-2xl mx-auto text-lg font-light leading-relaxed">
          No somos una empresa, somos una comunidad autogestionada. Aquí están las mentes y manos que hacen posible la Mesa de Rock y Metal de Mosquera.
        </p>
      </header>

      <div class="space-y-32">
        
        <section>
          <div class="flex items-center gap-4 mb-10">
            <h2 class="text-3xl font-black uppercase italic tracking-tighter">01. Gestión & Logística</h2>
            <div class="h-[2px] flex-grow bg-red-700/30"></div>
          </div>
          
          <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div v-for="i in 3" :key="i" class="group relative bg-[#111] p-8 border border-white/5 hover:border-red-700 transition-colors">
              <div class="absolute top-0 right-0 p-4 opacity-10 group-hover:opacity-100 transition-opacity">
                <span class="text-4xl italic font-black text-red-700">#0{{i}}</span>
              </div>
              <h3 class="text-xl font-black uppercase mb-1">Nombre Ejemplo {{i}}</h3>
              <p class="text-red-600 font-mono text-xs uppercase tracking-widest mb-4">Coordinador de Escenarios</p>
              <p class="text-gray-500 text-sm leading-relaxed">
                Encargado de la técnica y la coordinación de espacios para eventos en vivo.
              </p>
            </div>
          </div>
        </section>

        <section>
          <div class="flex items-center gap-4 mb-10">
            <div class="h-[2px] flex-grow bg-red-700/30"></div>
            <h2 class="text-3xl font-black uppercase italic tracking-tighter text-right">02. Prensa & Medios</h2>
          </div>
          
          <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
            <div v-for="i in 4" :key="i" class="relative overflow-hidden bg-white group aspect-square">
              <img :src="`https://i.pravatar.cc/400?img=${i+10}`" class="w-full h-full object-cover grayscale group-hover:scale-110 transition-transform duration-700" />
              <div class="absolute inset-0 bg-red-700/90 flex flex-col justify-end p-6 translate-y-full group-hover:translate-y-0 transition-transform duration-300">
                <h3 class="text-black font-black uppercase text-xl leading-none">Miembro {{i}}</h3>
                <p class="text-white font-mono text-xs mt-2 uppercase">Fotografía & Video</p>
              </div>
            </div>
          </div>
        </section>

        <section>
          <div class="flex items-center gap-4 mb-10">
            <h2 class="text-3xl font-black uppercase italic tracking-tighter">03. Alianzas & Bandas</h2>
            <div class="h-[2px] flex-grow bg-red-700/30"></div>
          </div>
          
          <div class="bg-red-700 p-10 md:p-16 flex flex-col md:flex-row gap-12 items-center">
            <div class="text-black max-w-md">
              <h3 class="text-5xl font-black uppercase leading-none mb-6 italic">Únete a la Mesa</h3>
              <p class="font-bold text-lg mb-8 uppercase tracking-tight">Estamos buscando líderes de bandas y gestores culturales de Mosquera.</p>
              <button class="bg-black text-white px-8 py-4 font-black uppercase hover:bg-white hover:text-black transition-all">
                Postularme ahora
              </button>
            </div>
            <div class="flex-grow grid grid-cols-2 gap-4">
              <div v-for="i in 4" :key="i" class="h-20 bg-black/20 backdrop-blur-sm border border-black/10 flex items-center justify-center italic font-black uppercase">
                Bandas Locales
              </div>
            </div>
          </div>
        </section>

      </div>

      <footer class="mt-32 text-center">
        <NuxtLink to="/" class="group inline-flex items-center gap-4 text-gray-500 hover:text-white transition-colors uppercase font-black tracking-widest">
          <span class="text-2xl group-hover:-translate-x-2 transition-transform">←</span>
          Volver al Inicio
        </NuxtLink>
      </footer>

    </div>
  </main>
</template>

<style scoped>
.text-stroke-white {
  -webkit-text-stroke: 1px white;
}

/* Efecto de grano sutil */
main::before {
  content: "";
  position: fixed;
  top: 0; left: 0; width: 100%; height: 100%;
  background-image: url('https://www.transparenttextures.com/patterns/stardust.png');
  opacity: 0.05;
  pointer-events: none;
  z-index: 50;
}
</style>