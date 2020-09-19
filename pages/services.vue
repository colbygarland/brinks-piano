<template>
    <div>
        <Content>
            <Container>
                <H1>Our Services</H1>
                <div class="prose">
                    <h3>Brink's Piano Works specializes in a number of different services.</h3>
                    <p>From piano tuning and repairs, to guitar sets-ups and fixing, Brink's is here to help you get your instruments back to playing as beautifully as they look.</p>
                </div>
            </Container>
        </Content>
       
       <ContentBackground id="piano">
           <Container>
               <H2 class="text-center">Pianos</H2>
           </Container>
       </ContentBackground>

       <Content>
           <Container>
               <div class="mb-6 lg:flex">
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Tunings" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano"
                            />
                        </div>
                   </div>
                  <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Repairs" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano2"
                            />
                        </div>
                   </div>
                   <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Climate Control Installation" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano3"
                            />
                        </div>
                   </div>
               </div>
               <div class="lg:flex">
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="String Replacement" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano"
                            />
                        </div>
                   </div>
                  <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Grande Piano Regulation" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano2"
                            />
                        </div>
                   </div>
                   <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Restoration" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano2"
                            />
                        </div>
                   </div>
               </div>
           </Container>
       </Content>

        <ContentBackground id="other">
           <Container>
               <H2 class="text-center">Other String Instruments</H2>
           </Container>
       </ContentBackground>

       <Content>
           <Container>
                <div class="mb-6 lg:flex">
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Instrument Set-ups" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="guitar"
                            />
                        </div>
                   </div>
                  <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card 
                                title="Instrument Repair" 
                                desc="Steve I need a write-up for this."
                                v-bind:image="piano2"
                            />
                        </div>
                   </div>
               </div>
           </Container>
       </Content>

       <ContentBackground id="other">
           <Container>
               <H2 class="text-center">Don't See What You Need?</H2>
               <div class="prose text-white text-center">
                   <p>Please send us a message using our <nuxt-link class="text-white" to="/contact"><span class="text-white font-bold">contact form.</span></nuxt-link></p>
               </div>
           </Container>
       </ContentBackground>

    </div>
</template>

<script>
    import piano from '~/assets/images/piano.jpg';
    import piano2 from '~/assets/images/piano3.jpg';
    import piano3 from '~/assets/images/keys.jpg';
    import guitar from '~/assets/images/guitar.jpg';

    export default {
        data() {
            return {
                piano,
                piano2,
                piano3,
                guitar,
            }
        }
    }
</script>