<template>
    <div>
        <div class="pt-16 lg:p-0 lg:flex lg:justify-between">
            <div class="text-center lg:text-left lg:w-1/2 lg:py-32 xl:py-64 lg:px-20">
                <div class="prose px-6 lg:p-0">
                    <div class="max-w-xl">
                        <h1 class="font-serif">Brink's Piano Works</h1>
                        <p>From piano tunings, to guitar set-ups, Brink's Piano Works is here to help you keep your instrument sounding as great as you play it.</p>
                    </div>
                </div>
                <div class="flex justify-center lg:justify-start mt-5 mb-5">
                    <nuxt-link to="/services" class="mr-5 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Our Services</nuxt-link>
                    <a href="" class="bg-transparent hover:bg-black hover:text-white text-black font-bold py-2 px-4 rounded font-serif">About Us</a>
                </div>
                <img class="mt-10 lg:hidden" src="~/assets/images/piano2.jpg" alt="Piano" />
            </div>
            <div class="hidden lg:w-1/2 lg:block lg:bg-cover lg:bg-no-repeat lg:bg-center lg:min-h-full" :style="{ backgroundImage: `url(${piano})` }"></div>
        </div>

        <div class="bg-gray-900 text-white py-10 px-6 lg:py-16">
            <div class="container mx-auto">
                <h2 class="text-center text-3xl lg:text-5xl font-serif font-bold">Our Services</h2>
            </div>
        </div>

        <div class="px-6 py-10 lg:py-16">
            <div class="container mx-auto">
                <div class="lg:flex">
                    <div class="mb-12 lg:mb-0 lg:px-4">
                        <h3 class="font-serif text-xl font-bold mb-4">Piano Tunings</h3>
                        <p>We tune pianos. We tune pianos. We tune pianos. We tune pianos. </p>
                        <nuxt-link to="/services" class="inline-block mt-3 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Learn more</nuxt-link>
                    </div>
                    <div class="mb-12 lg:mb-0 lg:px-4">
                        <h3 class="font-serif text-xl font-bold mb-4">Instrument Set Ups</h3>
                        <p>We tune pianos. We tune pianos. We tune pianos. We tune pianos. </p>
                        <nuxt-link to="/services" class="inline-block mt-3 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Learn more</nuxt-link>
                    </div>
                    <div class="mb-12 lg:mb-0 lg:px-4">
                        <h3 class="font-serif text-xl font-bold mb-4">Piano Tunings</h3>
                        <p>We tune pianos. We tune pianos. We tune pianos. We tune pianos. </p>
                        <nuxt-link to="/services" class="inline-block mt-3 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Learn more</nuxt-link>
                    </div>
                </div>
            </div>
        </div>

        <div class="bg-cover bg-no-repeat bg-center h-64 lg:h-50" :style="{ backgroundImage: `url(${piano})` }"></div>
    </div>
</template>

<script>
import piano from '~/assets/images/piano2.jpg';
export default {
    data() {
        return {
            piano,
        }
    }
}
</script>
