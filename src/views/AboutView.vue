<script>
export default {
  data() {
    return {
      activeTab: 1,
      contacts: [
        {
          id: 1,
          name: 'Email',
          value: 'dittosanzz02@gmail.com',
          icon: 'https://cdn-icons-png.flaticon.com/512/732/732200.png',
          link: 'mailto:ditto.alfiansyah@example.com'
        },
        {
          id: 2,
          name: 'WhatsApp',
          value: '+62 838-3753-4805',
          icon: 'https://cdn-icons-png.flaticon.com/512/733/733585.png',
          link: 'https://wa.me/6283837534805'
        },
        {
          id: 3,
          name: 'LinkedIn',
          value: 'Muhammad Ditto Alfiansyah',
          icon: 'https://cdn-icons-png.flaticon.com/512/174/174857.png',
          link: 'https://linkedin.com/in/muhammad-ditto'
        },
        {
          id: 4,
          name: 'GitHub',
          value: '@Idoo0oo',
          icon: 'https://cdn-icons-png.flaticon.com/512/25/25231.png',
          link: 'https://github.com/Idoo0oo'
        }
      ],
      tech: [
        {
          id: 1,
          name: 'HTML',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
          status: 'Advanced'
        },
        {
          id: 2,
          name: 'CSS',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/732/732190.png',
          status: 'Advanced'
        },
        {
          id: 3,
          name: 'PHP',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-php-2038871-1720084.png',
          status: 'Advanced'
        },
        {
          id: 4,
          name: 'Javascript',
          imageUrl: 'https://cdn.icon-icons.com/icons2/2415/PNG/512/javascript_original_logo_icon_146455.png',
          status: 'Intermediate'
        },
        {
          id: 5,
          name: 'Laravel',
          imageUrl: 'https://cdn.worldvectorlogo.com/logos/laravel-2.svg',
          status: 'Intermediate'
        },
        {
          id: 6,
          name: 'ExpressJS',
          imageUrl: 'https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/express.svg',
          status: 'beginner'
        },
        {
          id: 7,
          name: 'VueJS',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-vue-282497.png?f=webp',
          status: 'Beginner'
        },
        {
          id: 8,
          name: 'Figma',
          imageUrl: 'https://cdn.jsdelivr.net/npm/simple-icons@v10/icons/figma.svg',
          status: 'Advanced'
        },
        {
          id: 9,
          name: 'NodeJS',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-node-js-1174925.png',
          status: 'Beginner'
        },
        {
          id: 10,
          name: 'Tailwind',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/d/d5/Tailwind_CSS_Logo.svg',
          status: 'Intermediate'
        },
        {
          id: 11,
          name: 'Bootstrap',
          imageUrl: 'https://getbootstrap.com/docs/5.2/assets/brand/bootstrap-logo-shadow.png',
          status: 'Advanced'
        },
        {
          id: 12,
          name: 'ReactJS',
          imageUrl: 'https://cdn4.iconfinder.com/data/icons/logos-3/600/React.js_logo-512.png',
          status: 'Intermediate'
        }
      ],
      tools: [
        {
          id: 1,
          name: 'Git',
          imageUrl: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png',
          status: 'Version Control'
        },
        {
          id: 2,
          name: 'GitHub',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/25/25231.png',
          status: 'Git Hosting'
        },
        {
          id: 3,
          name: 'NPM',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-npm-3-1175132.png',
          status: 'Package Manager'
        },
        {
          id: 4,
          name: 'MySQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968313.png',
          status: 'Database'
        },
      ],
      // Data untuk section pacar
      girlfriend: {
        name: 'Bellaaaa',
        nickname: 'Bellskiee',
        photo: 'https://github.com/Idoo0oo/foto-bellskie/blob/main/bellskie.jpg?raw=true',
        anniversary: '30 Desember 2024',
        daysTogether: 200,
        profession: 'Matcha Loverrr',
        hobbies: ['Ngambek', 'Yapping', 'Matcha', 'Moodswing'],
        description: 'The woman who inspires me every day to be a better person. She brings colors to my black and white code.',
        quote: '"Behind every great developer is a woman who believes in him ❤️"',
        socialMedia: [
          {
            name: 'Instagram',
            icon: 'https://cdn-icons-png.flaticon.com/512/174/174855.png',
            link: 'https://instagram.com/anssdfzh',
            handle: '@anssdfzh'
          }
        ]
      },
      loveStats: [
        { label: 'Days Together', value: '200+', icon: '📅' },
        { label: 'Coffee Dates', value: '15+', icon: '☕' },
        { label: 'Ngambek', value: '999+', icon: '😤' },
        { label: 'Yapping', value: '999+', icon: '📢' }
      ]
    };
  }
}
</script>

<template>
  <!-- About Me Section -->
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Me &nbsp;
          <div class="h-[1px] w-32 bg-[#70dbff] md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-80 rounded-full mb-3 fadein-up"
            src="../assets/img/pp4.jpeg" alt="Foto">
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp; Hi everyone! My name is Muhammad Ditto Alfiansyah. I'm a web developer from Tangerang, Banten. I
            have 1 year of experience in back-end web development.
            I really enjoy what I do right now, in my opinion, creating programs is not just a job, but also an art that
            has
            aesthetic value
          </p>
          <p class="mb-3 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp; My job is to build your website to be functional and user-friendly yet still attractive.
            In addition, I provide a personal touch to your product and ensure that the website catches attention and is
            easy to use.
            My goal is to convey your message and identity in the most creative way. If you are interested in hiring me,
            please contact the listed contact.
          </p>
        </div>
      </section>
    </article>
  </div>

  <!-- My Heart Section (Pacar) -->
  <div
    class="bg-gradient-to-br from-[#1e1e1f] via-[#2a1e2a] to-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#ff69b4] rounded-3xl text-amber-50 mx-3 mb-5 relative overflow-hidden">
    <!-- Floating Hearts Animation -->
    <div class="absolute inset-0 pointer-events-none">
      <div class="floating-heart" style="left: 10%; animation-delay: 0s;">💖</div>
      <div class="floating-heart" style="left: 20%; animation-delay: 2s;">💕</div>
      <div class="floating-heart" style="left: 80%; animation-delay: 4s;">💝</div>
      <div class="floating-heart" style="left: 90%; animation-delay: 1s;">💗</div>
    </div>

    <article data-page="love" class="relative z-10">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          My Heart ❤️ &nbsp;
          <div class="h-[1px] w-32 bg-gradient-to-r from-[#ff69b4] to-[#70dbff] md:w-80 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section class="text-sm md:text-lg">
        <!-- Main Love Section -->
        <div class="flex flex-col gap-6 md:flex-row md:gap-8 md:items-center mb-8">
          <!-- Photo -->
          <div class="flex justify-center md:w-5/12">
            <div class="relative">
              <div class="absolute -inset-4 bg-gradient-to-r from-[#ff69b4] via-[#70dbff] to-[#ff69b4] rounded-full blur opacity-75 animate-pulse"></div>
              <img class="relative w-80 h-80 object-cover rounded-full mb-3 fadein-up border-4 border-white/20 shadow-2xl"
                :src="girlfriend.photo" :alt="girlfriend.name">
              <div class="absolute bottom-4 right-4 bg-red-500 text-white rounded-full w-12 h-12 flex items-center justify-center text-2xl animate-bounce">
                ❤️
              </div>
            </div>
          </div>
          
          <!-- Info -->
          <div class="md:w-7/12">
            <div class="mb-6 fadein-left fadeins-1">
              <h3 class="text-3xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-[#ff69b4] to-[#70dbff] mb-2">
                {{ girlfriend.name }}
              </h3>
              <p class="text-lg text-[#ff69b4] font-semibold mb-1">{{ girlfriend.nickname }} 💕</p>
              <p class="text-white/80 mb-4">{{ girlfriend.profession }}</p>
              <div class="flex items-center gap-4 text-sm text-white/60 mb-4">
                <span>👫 Since {{ girlfriend.anniversary }}</span>
                <span>•</span>
                <span>⏰ {{ girlfriend.daysTogether }} days together</span>
              </div>
            </div>
            
            <p class="mb-6 text-justify fadein-left fadeins-2 text-white/90 leading-relaxed">
              &nbsp; &nbsp; &nbsp; {{ girlfriend.description }}
            </p>
            
            <div class="bg-white/5 border-l-4 border-[#ff69b4] p-4 rounded-r-lg mb-6 fadein-left fadeins-3">
              <p class="italic text-[#ff69b4] text-center">{{ girlfriend.quote }}</p>
            </div>
          </div>
        </div>

        <!-- Love Stats -->
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-8 fadein-left fadeins-4">
          <div v-for="stat in loveStats" :key="stat.label" 
               class="bg-white/5 border border-[#ff69b4]/30 rounded-xl p-4 text-center hover:bg-white/10 transition-all duration-300 group">
            <div class="text-2xl mb-2 group-hover:scale-110 transition-transform duration-300">{{ stat.icon }}</div>
            <div class="text-2xl font-bold text-[#ff69b4] mb-1">{{ stat.value }}</div>
            <div class="text-xs text-white/60">{{ stat.label }}</div>
          </div>
        </div>

        <!-- Hobbies -->
        <div class="mb-8 fadein-left fadeins-5">
          <h4 class="text-xl font-semibold text-white mb-4 flex items-center">
            <span class="mr-2">🌟</span> Her Interests
          </h4>
          <div class="flex flex-wrap gap-3">
            <span v-for="hobby in girlfriend.hobbies" :key="hobby"
                  class="px-4 py-2 bg-gradient-to-r from-[#ff69b4]/20 to-[#70dbff]/20 border border-[#ff69b4]/30 rounded-full text-sm text-white hover:from-[#ff69b4]/30 hover:to-[#70dbff]/30 transition-all duration-300 cursor-pointer">
              {{ hobby }}
            </span>
          </div>
        </div>

        <!-- Social Media -->
        <div class="fadein-left fadeins-6">
          <h4 class="text-xl font-semibold text-white mb-4 flex items-center">
            <span class="mr-2">🔗</span> Connect with Her
          </h4>
          <div class="flex gap-4">
            <a v-for="social in girlfriend.socialMedia" :key="social.name"
               :href="social.link" target="_blank" rel="noopener noreferrer"
               class="flex items-center gap-3 bg-white/5 border border-[#ff69b4]/30 rounded-xl px-4 py-3 hover:bg-[#ff69b4]/10 transition-all duration-300 group">
              <img :src="social.icon" :alt="social.name" class="w-6 h-6 group-hover:scale-110 transition-transform duration-300">
              <div>
                <div class="text-white font-medium text-sm">{{ social.name }}</div>
                <div class="text-[#ff69b4] text-xs">{{ social.handle }}</div>
              </div>
            </a>
          </div>
        </div>

        <!-- Love Note -->
        <div class="mt-8 text-center bg-gradient-to-r from-[#ff69b4]/10 to-[#70dbff]/10 border border-[#ff69b4]/20 rounded-2xl p-6 fadein-left fadeins-7">
          <p class="text-white/80 text-lg font-light italic mb-4">
            "Professional yapping listener: Udah level expert ngangguk di waktu yang tepat ❤️"
          </p>
          <div class="text-[#ff69b4] font-semibold">— Ido 2024 —</div>
        </div>
      </section>
    </article>
  </div>

  <!-- Skills Section -->
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3 mb-5">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          <div class="h-[1px] w-10 bg-[#70dbff] md:w-20 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
          <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-[#70dbff] bg-[#70dbff] bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-[#70dbff] bg-[#70dbff] bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Tools</button>
            </li>
          </ul>
        </div>
        <div v-show="activeTab === 1">
          <div class="grid grid-cols-2 gap-4 pb-8 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tech" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-[#70dbff] px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div v-show="activeTab === 2">
          <div class="grid grid-cols-2 gap-4 pb-8 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tools" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-[#70dbff] px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>

  <!-- Contact CTA Section -->
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="contact">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          Let's Work Together &nbsp;
          <div class="h-[1px] w-32 bg-[#70dbff] md:w-80 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section class="text-center">
        <!-- CTA Text -->
        <div class="mb-8 fadein-left fadeins-1">
          <h3 class="text-xl md:text-2xl font-semibold text-white mb-4">
            Ready to bring your ideas to life?
          </h3>
          <p class="text-sm md:text-lg text-gray-300 max-w-3xl mx-auto">
            I'm always excited to work on new projects and collaborate with amazing people. 
            Whether you need a complete website, want to improve your existing project, or just have a question, 
            feel free to reach out!
          </p>
        </div>

        <!-- Contact Options -->
        <div class="grid grid-cols-1 gap-4 mb-8 md:grid-cols-2 lg:grid-cols-4 fadein-left fadeins-2">
          <div v-for="contact in contacts" :key="contact.id">
            <a :href="contact.link" target="_blank" rel="noopener noreferrer"
              class="contact-item flex flex-col items-center gap-3 rounded-xl border border-[#70dbff] px-4 py-6 hover:bg-[#70dbff] hover:bg-opacity-10 transition-all duration-300 group">
              <div class="flex h-12 w-12 items-center justify-center lg:h-14 lg:w-14">
                <img :alt="contact.name" loading="lazy" width="32" height="32" decoding="async"
                  class="contact-icon drop-shadow-xl transition-all duration-300 h-8 w-8 lg:h-10 lg:w-10"
                  :src="contact.icon" style="color: transparent;">
              </div>
              <div class="text-center">
                <div class="font-medium text-white text-sm md:text-base mb-1 group-hover:text-[#70dbff] transition-colors duration-300">
                  {{ contact.name }}
                </div>
                <div class="text-xs md:text-sm text-gray-400 group-hover:text-gray-300 transition-colors duration-300">
                  {{ contact.value }}
                </div>
              </div>
            </a>
          </div>
        </div>

        <!-- Primary CTA Button -->
        <div class="fadein-left fadeins-3">
          <a href="mailto:ditto.alfiansyah@example.com"
            class="inline-flex items-center gap-3 bg-[#70dbff] hover:bg-[#5bc3f0] text-black font-semibold px-8 py-4 rounded-xl transition-all duration-300 transform hover:scale-105 hover:shadow-lg hover:shadow-[#70dbff]/25">
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20">
              <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z"/>
              <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z"/>
            </svg>
            Start a Project
          </a>
        </div>

        <!-- Additional Info -->
        <div class="mt-8 pt-6 border-t border-[#383838] fadein-left fadeins-4">
          <p class="text-sm text-gray-400">
            Based in Tangerang, Banten • Available for freelance projects • 
            <span class="text-[#70dbff]">Response within 24 hours</span>
          </p>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.fadeins-3 {
  animation-delay: 1100ms;
}

.fadeins-4 {
  animation-delay: 1400ms;
}

.fadeins-5 {
  animation-delay: 1700ms;
}

.fadeins-6 {
  animation-delay: 2000ms;
}

.fadeins-7 {
  animation-delay: 2300ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}

.contact-icon {
  transition: transform 0.3s ease;
}

.contact-item:hover .contact-icon {
  transform: scale(1.2);
}

/* Romantic Animations */
.floating-heart {
  position: absolute;
  font-size: 1.5rem;
  animation: floatHeart 6s ease-in-out infinite;
  opacity: 0.7;
}

@keyframes floatHeart {
  0%, 100% {
    transform: translateY(100vh) rotate(0deg);
    opacity: 0;
  }
  10%, 90% {
    opacity: 0.7;
  }
  50% {
    transform: translateY(-20px) rotate(180deg);
    opacity: 1;
  }
}

/* Gradient text animation */
.gradient-text {
  background: linear-gradient(-45deg, #ff69b4, #70dbff, #ff69b4, #70dbff);
  background-size: 400% 400%;
  animation: gradientShift 3s ease infinite;
}

@keyframes gradientShift {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

/* Pulse effect for love stats */
.love-stat:hover {
  animation: lovePulse 0.6s ease-in-out;
}

@keyframes lovePulse {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.05);
  }
  100% {
    transform: scale(1);
  }
}
</style>