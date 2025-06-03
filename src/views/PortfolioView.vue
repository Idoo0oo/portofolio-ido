<script>
export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Personal Website Landing Page',
          imageUrl: 'landingpage',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'Html, Css, Javascript',
          github: 'https://github.com/Idoo0oo',
          demo: 'https://paellajaa.github.io/muhammad-ditto/'
        },
        {
          id: 2,
          name: 'CRUD Laravel 11',
          imageUrl: 'laravel',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'Laravel 11, Bootstrap',
          github: 'https://github.com/Idoo0oo',
          demo: 'https://github.com/Idoo0oo/CRUD-Laravel'
        },
        {
          id: 3,
          name: 'UI/UX E-Voting',
          imageUrl: 'uiux2',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'Figma',
          github: 'null',
          demo: 'null'
        },
        {
          id: 4,
          name: 'UI/UX Company Profile',
          imageUrl: 'uiux',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'Figma',
          github: 'null',
          demo: 'null'
        },
        {
          id: 5,
          name: 'Video Editing Four Fair',
          imageUrl: 'fourfair',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'Capcut',
          github: 'null',
          demo: 'null'
        },
        {
          id: 6,
          name: 'Video Editing Melaju',
          imageUrl: 'melaju',
          status: 'My personal website, I created this website to display my profile, skills and projects. As well as my place to try new technology.',
          tech: 'Capcut',
          github: 'null',
          demo: 'null'
        }
      ]
    };
  }
}
</script>
<template>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <h4>Past Project Experience</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-[#70dbff]">
            Explore the projects I've worked on so far</h4>
        </div>
      </header>
      <section>
        <div>
          <div class="grid grid-cols-1 gap-4 pb-32 md:grid-cols-3 md:gap-3 xl:grid-cols-3 xl:gap-3 2xl:gap-5 fade-zoom-in">
            <div v-for="item in items" :key="item.id">
              <div
                class="item-card flex flex-col gap-4 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-amber-50 px-5 py-5 h-full min-h-[400px]">
                
                <!-- Container gambar dengan ukuran tetap -->
                <div class="image-container w-full h-48 flex items-center justify-center overflow-hidden rounded-lg bg-gray-800">
                  <img 
                    alt="Project Image" 
                    loading="lazy" 
                    decoding="async" 
                    class="w-full h-full object-cover rounded-lg"
                    :src="'/img/portfolio-' + item.imageUrl + '.png'"
                  >
                </div>
                
                <!-- Content container yang mengisi sisa ruang -->
                <div class="flex flex-col flex-1 gap-3">
                  <!-- Title dengan tinggi tetap -->
                  <div class="title-text font-medium text-secondary text-lg leading-tight min-h-[3rem] flex items-center">
                    {{ item.name }}
                  </div>
                  
                  <!-- Description dengan tinggi fleksibel tapi terbatas -->
                  <div class="text-left text-sm text-[#c1c1c1] leading-relaxed flex-1 line-clamp-4">
                    {{ item.status }}
                  </div>
                  
                  <!-- Tech stack -->
                  <div class="text-sm text-[#70dbff] font-medium">
                    {{ item.tech }}
                  </div>
                  
                  <!-- Action buttons - selalu di bawah -->
                  <div class="flex justify-end mt-auto pt-3">
                    <div class="flex cursor-pointer items-center gap-3 text-primary">
                      <a v-if="item.github !== 'null'"
                        :href="item.github" target="_blank" rel="noreferrer"
                        title="View github repository" 
                        class="transition-all hover:text-accent p-2 hover:bg-gray-700 rounded-full">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22">
                          </path>
                        </svg>
                      </a>
                      <a v-if="item.demo !== 'null'" 
                        :href="item.demo" target="_blank" rel="noreferrer"
                        title="View finished project" 
                        class="transition-all hover:text-accent p-2 hover:bg-gray-700 rounded-full">
                        <svg stroke="currentColor"
                          fill="none" stroke-width="2" viewBox="0 0 24 24" stroke-linecap="round" stroke-linejoin="round"
                          height="18" width="18" xmlns="http://www.w3.org/2000/svg">
                          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                          <polyline points="15 3 21 3 21 9"></polyline>
                          <line x1="10" y1="14" x2="21" y2="3"></line>
                        </svg>
                      </a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.item-card {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.item-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
}

.item-card svg:hover {
  stroke: #70dbff;
}

/* Line clamp untuk membatasi text */
.line-clamp-4 {
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}

/* Memastikan semua card memiliki tinggi yang sama */
.item-card {
  display: flex;
  flex-direction: column;
}

/* Responsive image container */
.image-container {
  aspect-ratio: 16/9;
}
</style>