<template>
  <section class="relative min-h-screen w-full flex flex-col md:flex-row bg-[#0a0a0a] overflow-hidden">
    
    <div class="relative w-full md:w-1/2 h-[50vh] md:h-screen bg-red-900 flex items-center justify-center overflow-hidden border-b-8 md:border-b-0 md:border-r-8 border-white">
      <img 
        src="https://images.unsplash.com/photo-1493225255756-d9584f8606e9?q=80&w=2070" 
        class="absolute inset-0 w-full h-full object-cover opacity-40 mix-blend-overlay grayscale"
      />
      <div class="relative z-10 p-8">
        <img 
          src="/imagenes/inicio/logo_mesa_rock.jpg" 
          alt="Logo" 
          class="w-64 md:w-96 rounded-full shadow-[20px_20px_0px_0px_rgba(255,255,255,1)] border-4 border-white"
        />
      </div>
    </div>

    <div class="w-full md:w-1/2 flex items-center justify-center p-8 md:p-16">
      <div class="max-w-md">
        <span class="text-red-600 font-mono tracking-[0.3em] uppercase text-sm">Mosquera / Cundinamarca</span>
        
        <h1 class="text-white text-6xl md:text-8xl font-black uppercase leading-none mt-4 mb-8">
          ROCK <br/> <span class="italic">SANGRE</span> <br/> & METAL
        </h1>

        <p class="text-gray-400 text-lg mb-12 border-l-2 border-red-600 pl-4 font-light">
          Es un espacio donde convergen diversos integrantes de la escena del rock y metal, 
          busca trabajar transversal mente en las necesidades de la comunidad con especial 
          atención en los procesos musicales y sociales de sus integrantes.
        </p>

        <div class="grid grid-cols-1 gap-4">

          <NuxtLink
            to="/eventos"
            class="bg-white text-black px-8 py-4 font-black uppercase text-center hover:bg-red-600 hover:text-white transition-all duration-300 transform hover:-translate-y-1">
            Próximos Eventos
          </NuxtLink>
          <NuxtLink 
          to="/galeria" 
          class="px-8 py-4 border-2 border-white text-white font-black uppercase text-center hover:bg-white hover:text-black transition-all cursor-pointer inline-block">
          Galería Fotográfica
          </NuxtLink>
        </div>
      </div>
    </div>

    <div class="absolute bottom-4 left-4 text-white/5 text-9xl font-black pointer-events-none select-none">
      MESA
    </div>
  </section>
</template>