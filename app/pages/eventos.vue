<template>
  <section id="eventos" class="bg-black py-24 relative overflow-hidden">
    <div class="absolute top-0 left-1/2 -translate-x-1/2 w-full h-px bg-gradient-to-r from-transparent via-red-700 to-transparent"></div>

    <div class="container mx-auto px-6">
      
      <div class="mb-16 flex flex-col md:flex-row md:items-end justify-between gap-6">
        <div>
          <h2 class="text-6xl md:text-8xl font-black uppercase tracking-tighter text-white">
            PRÓXIMOS <br/> <span class="text-red-700 italic">ASALTOS</span>
          </h2>
        </div>
        <p class="text-gray-500 font-mono uppercase tracking-widest text-sm">
          // Calendario Oficial 2024 - 2025
        </p>
      </div>

      <div class="space-y-4">
        
        <div class="event-card group">
          <div class="date-box">
            <span class="day">15</span>
            <span class="month">MAR</span>
          </div>
          <div class="event-info">
            <h3 class="event-title text-white">MOSQUERA EXTREMA VOL. 3</h3>
            <p class="event-desc">Lugar: Auditorio Municipal • 4:00 PM</p>
          </div>
          <div class="event-status">
            <span class="status-badge bg-red-700 animate-pulse">PRÓXIMO</span>
            <button class="ticket-btn">INFO</button>
          </div>
        </div>

        <div class="event-card group border-white/10 opacity-80">
          <div class="date-box">
            <span class="day">22</span>
            <span class="month">ABR</span>
          </div>
          <div class="event-info">
            <h3 class="event-title text-white">TALLER DE GESTIÓN CULTURAL</h3>
            <p class="event-desc">Lugar: Biblioteca San Juan Bosco</p>
          </div>
          <div class="event-status">
            <span class="status-badge border border-white/20">AGENDADO</span>
            <button class="ticket-btn">INFO</button>
          </div>
        </div>

        <div class="py-10 flex items-center gap-4">
          <span class="text-gray-600 font-black uppercase tracking-widest text-xs">EVENTOS FINALIZADOS</span>
          <div class="h-px flex-grow bg-white/10"></div>
        </div>

        <div class="event-card group border-white/5 opacity-50 grayscale hover:grayscale-0 transition-all">
          <div class="date-box border-gray-800 text-gray-600">
            <span class="day font-light italic text-2xl">05</span>
            <span class="month text-[10px]">DIC</span>
          </div>
          <div class="event-info">
            <h3 class="text-xl font-bold uppercase text-gray-400">ROCK AL PARQUE MOSQUERA</h3>
            <p class="text-xs text-gray-600 uppercase tracking-widest">Finalizado con éxito • 2000 Asistentes</p>
          </div>
          <div class="event-status">
            <span class="text-red-900 font-black italic uppercase text-2xl rotate-12">CUMPLIDO</span>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
.event-card {
  @apply flex flex-col md:flex-row items-center gap-6 p-6 border-b-2 border-white/5 
         hover:bg-white/5 transition-all duration-300 relative overflow-hidden;
}

.date-box {
  @apply w-20 h-20 border-2 border-red-700 flex flex-col items-center justify-center 
         font-black transition-transform group-hover:scale-110 group-hover:bg-red-700 group-hover:text-black;
}

.date-box .day { @apply text-3xl leading-none; }
.date-box .month { @apply text-xs tracking-widest; }

.event-info { @apply flex-grow text-center md:text-left; }
.event-title { @apply text-2xl md:text-4xl font-black uppercase italic tracking-tighter; }
.event-desc { @apply text-gray-500 font-mono text-sm uppercase mt-1; }

.event-status { @apply flex items-center gap-4; }

.status-badge { @apply px-3 py-1 text-[10px] font-black uppercase tracking-widest text-white; }

.ticket-btn {
  @apply px-6 py-2 bg-white text-black font-black uppercase text-xs 
         hover:bg-red-700 hover:text-white transition-colors;
}
</style>