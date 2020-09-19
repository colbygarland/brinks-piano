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
                    <nuxt-link to="/about" class="bg-transparent hover:bg-black hover:text-white text-black font-bold py-2 px-4 rounded font-serif">About Us</nuxt-link>
                </div>
                <img class="mt-10 lg:hidden" :src="piano" alt="Piano" />
            </div>
            <div class="hidden lg:w-1/2 lg:block lg:bg-cover lg:bg-no-repeat lg:bg-center lg:min-h-full" :style="{ backgroundImage: `url(${piano})` }"></div>
        </div>

        <ContentBackground>
            <Container>
                <H2 class="text-center">Our Services</H2>
            </Container>
        </ContentBackground>

        <div class="px-6 py-10 lg:py-16">
            <div class="container mx-auto">
                <div class="lg:flex">
                    <div class="mb-12 lg:mb-0 lg:px-4">
                        <h3 class="font-serif text-xl font-bold mb-4">Pianos</h3>
                        <p>We offer a wide variety of piano services, from tuning, to string replacements, to Grand Piano Regulation.</p>
                        <nuxt-link to="/services#piano" class="inline-block mt-3 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Learn more</nuxt-link>
                    </div>
                    <div class="mb-12 lg:mb-0 lg:px-4">
                        <h3 class="font-serif text-xl font-bold mb-4">Instrument Set Ups</h3>
                        <p>From violins to guitars, and all in between, we pride ourselves in our ability to set up your instruments.</p>
                        <nuxt-link to="/services#other" class="inline-block mt-3 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Learn more</nuxt-link>
                    </div>
                    <div class="mb-12 lg:mb-0 lg:px-4">
                        <h3 class="font-serif text-xl font-bold mb-4">Instrument Repairs</h3>
                        <p>Pianos, guitars, you name it! Brinks Piano Works can repair your instrument.</p>
                        <nuxt-link to="/services#other" class="inline-block mt-3 bg-black hover:bg-gray-700 text-white font-bold py-2 px-4 rounded font-serif">Learn more</nuxt-link>
                    </div>
                </div>
            </div>
        </div>

        <div class="lg:flex">
            <div class="lg:w-1/3 h-50 bg-center bg-cover bg-no-repeat" :style="{ backgroundImage: `url(${piano2})` }"></div>
            <div class="lg:w-1/3 h-50 bg-center bg-cover bg-no-repeat" :style="{ backgroundImage: `url(${piano3})` }"></div>
            <div class="lg:w-1/3 h-50 bg-center bg-cover bg-no-repeat" :style="{ backgroundImage: `url(${piano4})` }"></div>
        </div>
    </div>
</template>

<script>
import piano from '~/assets/images/piano.jpg';
import piano2 from '~/assets/images/piano3.jpg';
import piano3 from '~/assets/images/piano-with-antlers.jpg';
import piano4 from '~/assets/images/keys.jpg';
export default {
    data() {
        return {
            piano,
            piano2,
            piano3,
            piano4,
        }
    }
}
</script>
