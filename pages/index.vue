<template>
  <div>
    <div class="flex flex-col w-screen min-h-screen bg-gray-200 bg-opacity-80">
      <div class="flex flex-row w-screen mt-2 mb-16 justify-between">
        <a href="/" class="text-2xl font-bold mx-4 justify-center">Vatsal Baherwani</a>
        <div class="flex flex-row mx-4 justify-evenly">
          <a target="_blank" href="https://www.github.com/vatsal0" class="rounded-full bg-purple-800 mx-1 w-10 h-10 flex flex-row justify-center items-center">
            <GithubIcon fillColor="#FFFFFF" :size="32"/>
          </a>
          <a target="_blank" href="https://www.linkedin.com/in/vatsal-baherwani" class="rounded-full bg-blue-800 mx-1 w-10 h-10 flex flex-row justify-center items-center">
            <LinkedinIcon fillColor="#FFFFFF" :size="32"/>
          </a>
          <a target="_blank" href="mailto:vatsalbaherwani@gmail.com" class="rounded-full bg-red-800 mx-1 w-10 h-10 flex flex-row justify-center items-center">
            <EmailIcon fillColor="#FFFFFF" :size="32"/>
          </a>
        </div>
      </div>
      <div class="flex flex-col sm:flex-row justify-center items-center w-screen my-6">
        <img src="https://avatars.githubusercontent.com/u/34689545" class="rounded-full max-w-sm"/>
        <div class="p-4 flex flex-col flex-shrink items-start min-w-md max-w-md">
          <p class="text-6xl font-bold mb-4">Hi, I'm Sal</p>
          <p class="text-xl mb-2">
            I'm a computer science student interested in machine learning and quantitative analysis. 
            I graduated from the Academy of Technology and Computer Science at 
            <a target="_blank" href="https://www.niche.com/k12/bergen-county-academies-hackensack-nj/" class="text-blue-500 hover:underline">Bergen County Academies</a> 
            in 2021 and am now majoring in computer science at the 
            <a target="_blank" href="https://www.umd.edu/" class="text-blue-500 hover:underline">University of Maryland</a>.
          </p>
          <p class="text-lg font-bold">Click on the links below to learn more about me!</p>
        </div>
      </div>
      <div class="flex flex-row justify-center items-start w-screen">
        <a href="#experience" class="bg-yellow-500 bg-opacity-80 rounded-xl py-4 px-2 w-40 mx-4 hover:bg-yellow-600 shadow-md transition ease-in duration-200 flex justify-center">
          <p class="text-xl text-white">Experience</p>
        </a>
        <a href="#projects" class="bg-green-500 bg-opacity-80 rounded-xl py-4 px-2 w-40 mx-4 hover:bg-green-600 shadow-md transition ease-in duration-200 flex justify-center">
          <p class="text-xl text-white">Projects</p>
        </a>
        <a href="#contact" class="bg-purple-500 bg-opacity-80 rounded-xl py-4 px-2 w-40 mx-4 hover:bg-purple-600 shadow-md transition ease-in duration-200 flex justify-center">
          <p class="text-xl text-white">Contact</p>
        </a>
      </div>
    </div>
    <div id="experience" class="flex flex-col w-screen min-h-screen bg-yellow-100 bg-opacity-80">
      I want a daughter like nicky oh man i promise i turne her to a monster but no menages
    </div>
    <div id="projects" class="flex flex-col w-screen min-h-screen bg-green-100 bg-opacity-80">
      I want a daughter like nicky oh man i promise i turne her to a monster but no menages
    </div>
    <div id="contact" class="flex flex-col w-screen h-40 bg-purple-100 bg-opacity-80">
      I want a daughter like nicky oh man i promise i turne her to a monster but no menages
    </div>
  </div>
</template>

<script>
import GithubIcon from 'vue-material-design-icons/Github.vue'
import LinkedinIcon from 'vue-material-design-icons/Linkedin.vue'
import EmailIcon from 'vue-material-design-icons/Email.vue'

export default {
  components: {
    GithubIcon,
    LinkedinIcon,
    EmailIcon
  }
}
</script>

<style>
  html{
    scroll-behavior:smooth;
    overflow: scroll;
    overflow-x: hidden;
  }
  ::-webkit-scrollbar {
      width: 0;  /* Remove scrollbar space */
      background: transparent;  /* Optional: just make scrollbar invisible */
  }
  .min-w-md {
    min-width: 28rem;
  }
</style>
