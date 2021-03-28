<template>
  <div class="min-h-screen bg-white text-black p-4">
      <div class="flex justify-between items center mb-4">
        <h2 class="text-header">About</h2>
        <nuxt-link to="/">
            <svg class="close-header" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path></svg>
        </nuxt-link>
      </div>
      <div class="flex flex-col lg:flex-row">
          <div class="w-full lg:w-2/3">
            <p class="paragraph">
                Hi, I'm Andikha Dian Nugraha, a Web Developer and UI/UX Enthusiast from Indonesia. Yeah, the Jakarta City, where I find a life partner who is with me from the beginning until now and "I'll do my best." Anyway...
            </p>
            <p class="paragraph mt-4">
                I have been a Full Stack developer for more than 2 years. In 2019, I graduated from the University of Indraprasta PGRI, where I learned to create interactive & dynamic websites with HTML, CSS, PHP and JavaScript. Currently, I build rich single-page web applications with Vue.js and Node.js.
            </p>
            <p class="paragraph mt-4">
                When I'm not coding, I learn and try to build a UI / UX Design to get me in the mood to try the results into code
                :D
            </p>
            <p class="paragraph mt-4">
                You can find me on this social media:
            </p>
           <social theme="light" align="left" class="mt-2" /> 
        </div>
        <div class="my-5 lg:my-0 lg:mx-5"></div>
        <div class="w-full lg:w-1/3 border-2 border-black p-4"></div>
      </div>
  </div>
</template>

<script>
import Social from '../components/Social.vue'
export default {
  components: { Social },
    
}
</script>

<style>

</style>