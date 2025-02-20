<template>
<div class="h-full p-8">
        <div class="bg-white rounded-lg  w-full xs:w-full sm:w-full md:w-[60%] lg:w-1/2 mx-auto my-auto shadow-xl pb-8">
            <div x-data="{ openSettings: false }" class="absolute right-12 mt-4 rounded">
                
            </div>
            <div class="w-full h-[250px]">
                <img src="/public/restusatyaw banner.webp" class="w-full h-full rounded-tl-lg rounded-tr-lg">
            </div>
            <div class="flex flex-col items-center -mt-20">
                <img src="/public/restusatyaw.webp" class="w-[120px] h-[120px] border-4 border-white rounded-full object-cover object-top">
                <div class="flex items-center space-x-2 mt-2">
                    <p class="text-2xl capitalize">{{ profile?.name }}</p>
                    <span class="bg-blue-500 rounded-full p-1" title="Verified">
                        <svg xmlns="http://www.w3.org/2000/svg" class="text-gray-100 h-2.5 w-2.5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="4" d="M5 13l4 4L19 7"></path>
                        </svg>
                    </span>
                </div>
                <p class="text-sm text-gray-600 mt-2">Web Developer | Based in {{ profile?.address }}</p>
            </div>
            <div class="w-full p-6 text-center">
                <p>Hy there !, My name restusasatyaw</p>
                <p class="mt-4 text-gray-700 ">Building <span class="font-semibold hover:underline hover:bg-black hover:text-white hover:capitalize hover:p-2">powerful and visually stunning websites</span> is my passion. I love crafting <span class="font-semibold hover:underline hover:bg-black hover:text-white hover:capitalize hover:p-2">clean, minimal, and functional digital products</span> while constantly exploring new ideas and innovations.</p>
                
                <p class="mt-4 text-gray-700">Beyond coding, I’m also an investor and enjoy writing about <span class="font-semibold hover:underline hover:bg-black hover:text-white hover:capitalize hover:p-2">tech development and place reviews</span>.</p>
                
                <a :href="`mailto:${profile.email}`" class="mt-6 inline-block px-4 py-2 underline">gmail@kadekrestusatyawardana</a>
            </div>
            <div class="flex-1 flex flex-col items-center lg:items-center justify-center px-2 mt-2">
                <div class="flex items-center gap-2 mt-2">
                    <a :href="profile?.instagram_link" class="flex items-center border border-gray-400 min-h-[40px]  hover:bg-blue-700 text-gray-100 px-4 py-2 rounded-2xl text-sm space-x-2 transition duration-100">
                        <img src="/public/instagram.webp" alt="" class="w-[20px]" srcset="">
                    </a>
                    <a :href="profile?.facebook_link" class="flex items-center border border-gray-400 min-h-[40px]  hover:bg-blue-700 text-gray-100 px-4 py-2 rounded-2xl text-sm space-x-2 transition duration-100">
                        <img src="/public/facebook.webp" alt="" class="w-[20px]" srcset="">
                    </a>
                    <a :href="profile?.linkendin_link" class="flex items-center border border-gray-400 min-h-[40px]  hover:bg-gray-500 text-gray-100 px-4 py-2 rounded-2xl text-sm space-x-2 transition duration-100">
                        <img src="/public/linkendin.webp" alt="" class="w-[20px]" srcset="">
                    </a>
                    <a :href="profile?.github_link" class="flex items-center border border-gray-400 min-h-[40px]  hover:bg-black  text-gray-100 px-4 py-2 rounded-2xl text-sm space-x-2 transition duration-100">
                        <img src="/public/github.webp" alt="" class="w-[20px] rounded-4xl" srcset="">
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
useHead({
  title: 'Web Developer based in Bali | Kadek Restu Satya Wardana',
  meta: [
    { name: 'description', content: '.' }
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [ { innerHTML: 'console.log(\'Hello world\')' } ]
})
const profile = ref({
    "name": "kadek restu satya wardana",
    "email":"kadekrestusatyawardana@gmail.com",
    "position": "web developer",
    "github_link": "https://github.com/restusatyaw",
    "instagram_link": "https://www.instagram.com/kdrestusat_/?locale=en",
    "facebook_link": "https://github.com/restusatyaw",
    "linkendin_link": "https://id.linkedin.com/in/kadek-restu-satya-wardana-3467b4297",
    "total_project": "80+",
    "address":"Denpasar, Bali"
    })
</script>
<style>
    
</style>