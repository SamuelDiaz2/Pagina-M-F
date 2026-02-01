<template>
  <section class="relative bg-[#080808] py-20 overflow-hidden">
    <div class="absolute top-0 right-0 opacity-[0.02] pointer-events-none select-none">
      <h2 class="text-[15rem] font-black leading-none">ROCK</h2>
    </div>

    <div class="container mx-auto px-6 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
        
        <div class="relative group">
          <div class="absolute -bottom-4 -left-4 w-full h-full border-2 border-red-700 z-0 transition-transform group-hover:translate-x-2 group-hover:translate-y-2"></div>
          
          <div class="relative z-100 overflow-hidden">
            <img 
              src="https://periodicodelmeta.com/wp-content/uploads/2021/07/bandas-rock.jpg" 
              alt="Cultura Rock Mosquera" 
              class="w-full h-[500px] object-cover grayscale hover:grayscale-0 transition-all duration-700 shadow-2xl"
            />
            <div class="absolute inset-0 bg-red-700/10 opacity-0 group-hover:opacity-100 transition-opacity"></div>
          </div>

          <div class="absolute -bottom-6 -right-6 bg-red-700 text-white p-6 shadow-xl hidden md:block">
            <p class="font-black text-2xl uppercase italic tracking-tighter">Desde el 2020</p>
          </div>
        </div>

        <div class="flex flex-col space-y-8">
          <div>
            <span class="text-red-600 font-mono tracking-[0.4em] uppercase text-sm">Nuestra Esencia</span>
            <h2 class="text-5xl md:text-7xl font-black text-white uppercase tracking-tighter mt-2 leading-none">
              Más que música, <br/> 
              <span class="italic text-transparent text-stroke-white">una mesa para todos</span>
            </h2>
          </div>

          <p class="text-gray-400 text-lg md:text-xl leading-relaxed font-light border-l-4 border-red-700 pl-6">
            La Mesa de Rock y Metal de Mosquera nace como un espacio de gestión, unión y 
            resistencia cultural. Somos el punto de encuentro para bandas, artistas y 
            seguidores que creen en el poder del ruido consciente.
          </p>

          <div class="space-y-4">
            <div class="flex items-start gap-4">
              <div class="mt-2 w-3 h-3 bg-red-700 rotate-45"></div>
              <p class="text-white font-bold uppercase tracking-widest text-sm">Fomento de la cultura local</p>
            </div>
            <div class="flex items-start gap-4">
              <div class="mt-2 w-3 h-3 bg-red-700 rotate-45"></div>
              <p class="text-white font-bold uppercase tracking-widest text-sm">Gestión de espacios dignos para el metal</p>
            </div>
            <div class="flex items-start gap-4">
              <div class="mt-2 w-3 h-3 bg-red-700 rotate-45"></div>
              <p class="text-white font-bold uppercase tracking-widest text-sm">Unión de la escena alternativa de Mosquera</p>
            </div>
          </div>

          <div class="pt-6">
            <NuxtLink to="/nosotros" class="inline-block bg-white text-black px-10 py-4 font-black uppercase tracking-widest hover:bg-red-700 hover:text-white transition-all duration-300 transform hover:-translate-y-1 shadow-[8px_8px_0px_0px_rgba(185,28,28,1)]">
              Conoce al Equipo
            </NuxtLink>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<style scoped>
.text-stroke-white {
  -webkit-text-stroke: 1px rgba(255,255,255,0.5);
}
</style>