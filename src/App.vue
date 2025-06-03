<template>
  <!-- component -->
  <!-- This is an example component -->
  <div class="max-w-7xl mx-auto flex flex-col relative">

    <nav class="max-w-7xl px-5 md:fixed top-0 z-[98] w-screen backdrop-blur-md bg-[#121212] bg-opacity-80">
      <div class="container mx-auto flex flex-wrap items-center justify-between">
        <button @click="redirectToHome" class="flex">
          <span class="self-center text-lg text-[#70dbff] font-semibold whitespace-nowrap fadein-bot hover:text-amber-100">MuhammadDitto();</span>
        </button>
        <div class="flex md:order-2 fadein-bot">
          <a href="https://github.com/Idoo0oo"><img class="w-10 rounded" src="https://seeklogo.com/images/G/github-logo-2E3852456C-seeklogo.com.png" alt="github"></a>
        </div>
        <div class="hidden md:flex justify-between items-center w-full md:w-auto md:order-1" id="mobile-menu-3">
          <ul class="flex-col md:flex-row flex md:space-x-8 mt-4 md:mt-0 md:text-sm md:font-medium">
            <li>
              <router-link to="/"
                class="nav-item fadein-bot text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0"
                aria-current="page">Home</router-link>
            </li>
            <li>
              <router-link to="/about"
                class="nav-item fadein-bot fadein-1 text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0">About</router-link>
            </li>
            <li>
              <router-link to="/portfolio"
                class="nav-item fadein-bot fadein-2 text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0">Portfolio</router-link>
            </li>
            <li>
              <router-link to="/blog"
                class="nav-item fadein-bot fadein-3 text-gray-700 hover:bg-gray-50 border-b border-gray-100 md:hover:bg-transparent md:border-0 block pl-3 pr-4 py-2 md:hover:text-gray-500 md:p-0 blog">Blog</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <div class="md:mt-[100px]">
      <router-view />
    </div>
  </div>
  <footer class="block md:hidden fixed bottom-0 left-0 right-0 rounded-t-3xl border border-[#383838] bg-[#121212] bg-opacity-80 backdrop-blur-md backdrop-opacity-90">
  <nav class="flex justify-around py-4 text-xs">
    <router-link to="/" class="mobile-nav-item text-gray-300 hover:text-white">Home</router-link>
    <router-link to="/about" class="mobile-nav-item text-gray-300 hover:text-white">About</router-link>
    <router-link to="/portfolio" class="mobile-nav-item text-gray-300 hover:text-white">Portfolio</router-link>
    <router-link to="/blog" class="mobile-nav-item text-gray-300 hover:text-white">Blog</router-link>
  </nav>
</footer>
</template>

<script>
export default {
  methods: {
    redirectToHome() {
      this.$router.push('/')
    }
  },
}
</script>

<style>
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

::-webkit-scrollbar {
  width: 5px; /* for vertical scrollbar */
  height: 5px; /* for horizontal scrollbar */
}

::-webkit-scrollbar-track {
  background: hsl(240, 1%, 17%);
  border-radius: 5px;
}

::-webkit-scrollbar-thumb {
  background: #70dbff;
  border-radius: 5px;
}

::-webkit-scrollbar-button { width: 20px; }

body {
  font-family: 'Poppins', sans-serif;
  background: hsl(0, 0%, 7%);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  transition: color 0.3s;
}

/* Hover effect untuk desktop nav items */
.nav-item {
  position: relative;
  display: inline-block;
  transition: color 0.3s ease;
}

.nav-item::before {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 50%;
  width: 0;
  height: 3px;
  background-color: #70dbff;
  border-radius: 2px;
  transition: all 0.3s ease;
  transform: translateX(-50%);
}

/* Hover effect hanya untuk item yang tidak aktif */
.nav-item:not(.router-link-exact-active):hover::before {
  width: 100%;
}

.nav-item:not(.router-link-exact-active):hover {
  color: #70dbff !important;
}

/* Active state styling */
nav a.router-link-exact-active {
  display: inline-flex;
  flex-direction: column;
  color: white;
  transition: color 0.3s;
  position: relative;
}

nav a.router-link-exact-active::after {
  display: inline-block;
  content: "";
  margin-top: 0.08em;
  width: 100%;
  height: 4px;
  border-radius: 2px;
  background-color: #70dbff;
}

nav a.router-link-exact-active:hover {
  color: white;
}

/* Mobile nav hover effect */
.mobile-nav-item {
  position: relative;
  display: inline-block;
  transition: color 0.3s ease;
}

.mobile-nav-item::before {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 50%;
  width: 0;
  height: 2px;
  background-color: #70dbff;
  border-radius: 2px;
  transition: all 0.3s ease;
  transform: translateX(-50%);
}

/* Hover effect hanya untuk item yang tidak aktif */
.mobile-nav-item:not(.router-link-exact-active):hover::before {
  width: 100%;
}

.mobile-nav-item:not(.router-link-exact-active):hover {
  color: #70dbff !important;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(-100%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}
</style>