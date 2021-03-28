<template>
  <div class="container relative">
    <div class="p-4">
      <div class="mb-8">
        <h1 class="text-gray-500 text-5xl md:text-8xl font-bold">Andikha Dian</h1>
        <p class="text-md md:text-2xl mt-3">Software Engineer & UI/UX Enthusiast from Indonesia, Jakarta</p>
      </div>
      <div class="flex flex-col md:flex-row items-center justify-center mb-8">
        <nuxt-link to="/about" class="w-full mb-2 md:mb-0 md:mr-8"> 
          <button class="btn-primary w-full mb-2 md:mb-0 md:mr-8">
            <span class="text-btn-heading">About</span>
            <span class="text-btn-shortcut">Ctrl + A</span>
          </button>
        </nuxt-link>
        <nuxt-link to="/skills" class="w-full mb-2 md:mb-0 md:mr-8">
          <button class="btn-primary w-full mb-2 md:mb-0 md:mr-8">
            <span class="text-btn-heading">Skills</span>
            <span class="text-btn-shortcut">Ctrl + W</span>
          </button>
        </nuxt-link>
        <nuxt-link to="/projects" class="w-full mb-2 md:mb-0 md:mr-8">
          <button class="btn-primary w-full mb-2 md:mb-0 md:mr-8">
            <span class="text-btn-heading">Project</span>
            <span class="text-btn-shortcut">Ctrl + P</span>
          </button>
        </nuxt-link>
        <nuxt-link to="contact" class="w-full">
          <button class="btn-primary w-full">
            <span class="text-btn-heading">Contact</span>
            <span class="text-btn-shortcut">Ctrl + C</span>
          </button>
        </nuxt-link>
      </div>
      <social theme="light" align="center" />
    </div>
      <p class="absolute bottom-2 text-xs underline">Copyright © 2021. All Rights Reserved.</p>
  </div>
</template>

<script>
import social from '../components/Social.vue'
export default {
  transition: "page",
  components: {
    social
  }
}
</script>

<style>
.page-enter-active {
  animation: acrossIn .35s ease-out both;
} 

/* .page-leave-active {
  animation: accrossOut .35s ease-in both;
}  */

@keyframes acrossIn {
  0% {
    transform: translate3d(0, 100%, 0);
  }
  100% {
    transform: translate3d(0, 0, 0);
  }
}

@keyframes acrossOut {
  0% {
    transform: translate3d(100%, 0, 0);
  }
  100% {
    transform: translate3d(0, -100%, 0);
  }
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.btn-primary {
  @apply py-4 px-8 border-2 border-black bg-transparent flex flex-col justify-center items-center focus:outline-none;
}

.text-btn-heading {
  @apply text-lg font-bold;
}

.text-btn-shortcut {
  @apply text-sm font-light italic;
}
</style>
