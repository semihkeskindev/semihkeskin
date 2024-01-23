<script setup>
import Layout from '../Layout.vue'
import {Head} from '@inertiajs/vue3'
</script>

<script>
export default {
  data() {
    return {
      name: 'Semih Keskin',
      title: 'Software Developer',
      avatarImageLink: 'https://avatars.githubusercontent.com/u/32278879',
      githubLink: 'https://github.com/semihkeskindev',
      linkedinLink: 'https://www.linkedin.com/in/semih-keskin/',
      instagramLink: 'https://www.instagram.com/semihkeskindev/',
      twitterLink: 'https://twitter.com/semihkeskindev',
      emailLink: 'mailto:semihkeskindev@gmail.com',
      mediumLink: 'https://medium.com/@semih.keskin',
    }
  },
}
</script>

<style scoped>
[data-radix-scroll-area-viewport] {
  scrollbar-width: none;
  -ms-overflow-style: none;
  -webkit-overflow-scrolling: touch;
}

[data-radix-scroll-area-viewport]::-webkit-scrollbar {
  display: none
}

.navbar-menu-list li[aria-disabled=true] a {
  pointer-events: none;
  cursor: default;
  opacity: .5;
}
</style>

<template>
  <Layout>
    <div class="lg:container mx-auto min-h-screen items-center flex">
      <div class=" self-center mx-auto rounded-2xl py-10 inset-x-0 px-8 bg-white min-w-[100px] max-w-max">
        <nav aria-label="Main" data-orientation="horizontal" dir="ltr"
             class="relative z-10 flex flex-col max-w-max flex-1 items-center justify-center gap-y-5">
          <div class="flex flex-row items-center gap-x-2 p-5 border-b rounded-full shadow-sm shadow-gray-300 mb-10">
            <div><span class="relative flex h-16 w-16 shrink-0 overflow-hidden rounded-full"><img
                class="aspect-square h-full w-full" alt="avatar"
                :src="avatarImageLink"></span></div>
            <div><p class="font-bold text-xl mono">{{ name}}</p>
              <p class="text-md mono font-light">{{ title }}</p></div>
          </div>
          <div style="position: relative;width: 100%;">
            <ul data-orientation="horizontal"
                class="navbar-menu-list group flex flex-col flex-1 list-none items-center justify-center space-x-1 gap-y-4 w-full px-4" dir="ltr">
              <li class="w-full"><a target="_blank"
                  class="shadow-sm shadow-gray-400 group inline-flex gap-x-2 h-9 w-full items-center justify-center rounded-md bg-white px-4 py-2 text-sm font-medium transition-colors hover:bg-stone-100 hover:text-stone-900 focus:bg-stone-100 focus:text-stone-900 focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-stone-100/50 data-[state=open]:bg-stone-100/50 cursor-pointer"
                  :href="githubLink">
                <svg data-v-75f1c265="" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-github"><path data-v-75f1c265="" d="M15 22v-4a4.8 4.8 0 0 0-1-3.5c3 0 6-2 6-5.5.08-1.25-.27-2.48-1-3.5.28-1.15.28-2.35 0-3.5 0 0-1 0-3 1.5-2.64-.5-5.36-.5-8 0C6 2 5 2 5 2c-.3 1.15-.3 2.35 0 3.5A5.403 5.403 0 0 0 4 9c0 3.5 3 5.5 6 5.5-.39.49-.68 1.05-.85 1.65-.17.6-.22 1.23-.15 1.85v4"></path><path data-v-75f1c265="" d="M9 18c-4.51 2-5-2-7-2"></path></svg>
                Github</a></li>
              <li class="w-full"><a target="_blank"
                  class="shadow-sm shadow-gray-400 group inline-flex gap-x-2 h-9 w-full items-center justify-center rounded-md bg-white px-4 py-2 text-sm font-medium transition-colors hover:bg-stone-100 hover:text-stone-900 focus:bg-stone-100 focus:text-stone-900 focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-stone-100/50 data-[state=open]:bg-stone-100/50 cursor-pointer"
                  :href="linkedinLink">
                <svg data-v-3ed5cb83="" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-linkedin"><path data-v-3ed5cb83="" d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect data-v-3ed5cb83="" width="4" height="12" x="2" y="9"></rect><circle data-v-3ed5cb83="" cx="4" cy="4" r="2"></circle></svg>
                Linkedin</a></li>
              <li class="w-full"><a target="_blank"
                  class="shadow-sm shadow-gray-400 group inline-flex gap-x-2 h-9 w-full items-center justify-center rounded-md bg-white px-4 py-2 text-sm font-medium transition-colors hover:bg-stone-100 hover:text-stone-900 focus:bg-stone-100 focus:text-stone-900 focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-stone-100/50 data-[state=open]:bg-stone-100/50 cursor-pointer"
                  :href="instagramLink">
                <svg data-v-3ed5cb83="" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-instagram"><rect data-v-3ed5cb83="" width="20" height="20" x="2" y="2" rx="5" ry="5"></rect><path data-v-3ed5cb83="" d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line data-v-3ed5cb83="" x1="17.5" x2="17.51" y1="6.5" y2="6.5"></line></svg>
                Instagram</a></li>
              <li class="w-full"><a target="_blank"
                  class="shadow-sm shadow-gray-400 group inline-flex gap-x-2 h-9 w-full items-center justify-center rounded-md bg-white px-4 py-2 text-sm font-medium transition-colors hover:bg-stone-100 hover:text-stone-900 focus:bg-stone-100 focus:text-stone-900 focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-stone-100/50 data-[state=open]:bg-stone-100/50 cursor-pointer"
                  :href="twitterLink">
                <svg data-v-877ffa9d="" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-twitter"><path data-v-877ffa9d="" d="M22 4s-.7 2.1-2 3.4c1.6 10-9.4 17.3-18 11.6 2.2.1 4.4-.6 6-2C3 15.5.5 9.6 3 5c2.2 2.6 5.6 4.1 9 4-.9-4.2 4-6.6 7-3.8 1.1 0 3-1.2 3-1.2z"></path></svg>
                Twitter</a></li>
              <li class="w-full"><a target="_blank"
                  class="shadow-sm shadow-gray-400 group inline-flex gap-x-2 h-9 w-full items-center justify-center rounded-md bg-white px-4 py-2 text-sm font-medium transition-colors hover:bg-stone-100 hover:text-stone-900 focus:bg-stone-100 focus:text-stone-900 focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-stone-100/50 data-[state=open]:bg-stone-100/50 cursor-pointer"
                  :href="emailLink">
                <svg data-v-877ffa9d="" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail"><rect data-v-877ffa9d="" width="20" height="16" x="2" y="4" rx="2"></rect><path data-v-877ffa9d="" d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"></path></svg>
                E-mail</a></li>
              <li class="w-full"><a target="_blank"
                  class="shadow-sm shadow-gray-400 group inline-flex gap-x-2 h-9 w-full items-center justify-center rounded-md bg-white px-4 py-2 text-sm font-medium transition-colors hover:bg-stone-100 hover:text-stone-900 focus:bg-stone-100 focus:text-stone-900 focus:outline-none disabled:pointer-events-none disabled:opacity-50 data-[active]:bg-stone-100/50 data-[state=open]:bg-stone-100/50 cursor-pointer"
                  :href="mediumLink">
                <svg width="20" viewBox="0 0 1043.63 592.71" class="cn co"><g data-name="Layer 2"><g data-name="Layer 1"><path d="M588.67 296.36c0 163.67-131.78 296.35-294.33 296.35S0 460 0 296.36 131.78 0 294.34 0s294.33 132.69 294.33 296.36M911.56 296.36c0 154.06-65.89 279-147.17 279s-147.17-124.94-147.17-279 65.88-279 147.16-279 147.17 124.9 147.17 279M1043.63 296.36c0 138-23.17 249.94-51.76 249.94s-51.75-111.91-51.75-249.94 23.17-249.94 51.75-249.94 51.76 111.9 51.76 249.94"></path></g></g></svg>
                Medium</a></li>

            </ul>
          </div>
          <div class="absolute left-0 bottom-full flex justify-center"></div>
        </nav>
      </div>
    </div>
  </Layout>
</template>