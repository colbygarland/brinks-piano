<template>
    <header class="bg-gray-100 py-4 shadow z-20 lg:sticky w-full">
        <div class="container mx-auto lg:flex lg:justify-between">
            <a href="/" class="block">
                <img class="h-24 lg:h-20 mx-auto" src="~/assets/images/brinks-piano-works-logo.svg" />
            </a>
            <nav class="">
                <div class="lg:hidden">
                    <div class="relative">
                        <div class="flex justify-center mt-5">
                            <!-- Mobile menu button-->
                            <button v-on:click="showMenu = !showMenu" class="inline-flex items-center justify-center p-2 rounded-md  hover:text-white hover:bg-gray-900 focus:outline-none focus:bg-gray-900 focus:text-white transition duration-150 ease-in-out" aria-label="Main menu" aria-expanded="false">
                                <!-- Icon when menu is closed. -->
                                <!-- Menu open: "hidden", Menu closed: "block" -->
                                <svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                                </svg>
                                <!-- Icon when menu is open. -->
                                <!-- Menu open: "block", Menu closed: "hidden" -->
                                <svg class="hidden h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                                </svg>
                            </button>
                        </div>
                    </div>
                </div>
                <div class="hidden lg:block flex-1 flex items-center justify-center sm:items-stretch sm:justify-start h-full">
                    <div class="flex h-full items-center">
                        <nuxt-link class="font-bold font-serif text-gray-600 hover:text-black text-lg ml-5 mr-5" to="/">Home</nuxt-link>
                        <nuxt-link class="font-bold font-serif text-gray-600 hover:text-black text-lg ml-5 mr-5" to="/about">About</nuxt-link>
                        <nuxt-link class="font-bold font-serif text-gray-600 hover:text-black text-lg ml-5 mr-5" to="/services">Services</nuxt-link>
                        <nuxt-link class="font-bold font-serif text-gray-600 hover:text-black text-lg ml-5 mr-5" to="/contact">Contact</nuxt-link>
                    </div>
                </div>
                <!--
                  Mobile menu, toggle classes based on menu state.

                  Menu open: "block", Menu closed: "hidden"
                -->
                <div v-show="showMenu" class="lg:hidden">
                    <div class="px-2 pt-2 pb-3">
                        <ul>
                            <li v-on:click="toggleMenu"><nuxt-link class="font-bold font-serif block px-3 py-2 rounded-md text-base text-gray-600 hover:text-white hover:bg-gray-900 font-medium focus:outline-none focus:text-white focus:bg-gray-900 transition duration-150 ease-in-out" to="/">Home</nuxt-link></li>
                            <li v-on:click="toggleMenu"><nuxt-link class="font-bold font-serif block px-3 py-2 rounded-md text-base text-gray-600 hover:text-white hover:bg-gray-900 font-medium focus:outline-none focus:text-white focus:bg-gray-900 transition duration-150 ease-in-out" to="/about">About</nuxt-link></li>
                            <li v-on:click="toggleMenu"> <nuxt-link class="font-bold font-serif block px-3 py-2 rounded-md text-base text-gray-600 hover:text-white hover:bg-gray-900 font-medium focus:outline-none focus:text-white focus:bg-gray-900 transition duration-150 ease-in-out" to="/services">Services</nuxt-link></li>
                            <li v-on:click="toggleMenu"><nuxt-link class="font-bold font-serif block px-3 py-2 rounded-md text-base text-gray-600 hover:text-white hover:bg-gray-900 font-medium focus:outline-none focus:text-white focus:bg-gray-900 transition duration-150 ease-in-out" to="/contact">Contact</nuxt-link></li>
                        </ul>
                        <div class="flex mt-4">
                            <a target="_blank" href="" class="inline-block h-6 w-6 ml-4 mr-4 opacity-50 hover:opacity-100">
                                <img src="~/assets/images/facebook.svg" alt="Brinks Piano Work On Facebook" />
                            </a>
                            <a target="_blank" href="" class="inline-block h-6 w-6 ml-4 mr-4 opacity-50 hover:opacity-100">
                                <img src="~/assets/images/instagram.svg" alt="Brinks Piano Work On Instagram" />
                            </a>
                        </div>
                    </div>
                </div>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    data() {
        return {
            showMenu: false,
        };
    },
    methods: {
        toggleMenu: function(){
            this.showMenu = false;
        }
    }
}
</script>
