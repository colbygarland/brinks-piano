<template>
    <div>
        <Content>
            <Container>
                <H1>Our Services</H1>
                <div class="prose">
                    <h3>
                        Brink's Piano Works specializes in a number of different
                        services.
                    </h3>
                    <p>
                        From piano tuning and repairs, to guitar sets-ups and
                        fixing, Brink's is here to help you get your instruments
                        back to playing as beautifully as they look.
                    </p>
                    <h4>Pricing</h4>
                    <p>
                        At Brink's Piano Works our prices are subject to change,
                        based on many factors including the condition of one's
                        piano.
                    </p>
                    <p>
                        I charge to travel by the kilometer, outside of my area.
                        The price is firm, but it doesn’t go up. I try to line
                        up more pianos in that area, so the travel bill can be
                        split between more people. Making it more cost effective
                        for everyone.
                    </p>
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
                                desc="Our tunings range in price depending on your needs and the piano. How long it has been since the last tuning, or even where it sits, pitch wise. Please contact me, and we will discuss prices."
                                v-bind:image="piano"
                            />
                        </div>
                    </div>
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card
                                title="Repairs"
                                desc="Repairs range in price and estimates will be provided beforehand, so there are no surprises in the fixing of your instruments. Whether it be guitar, piano, violin etc."
                                v-bind:image="piano2"
                            />
                        </div>
                    </div>
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card
                                title="Climate Control Installation"
                                desc="At Brink’s Piano works, we prefer preventative maintenance to huge repairs. So I recommend, and install, Dampp Chaser climate control systems in both upright and grand pianos. Contact me anytime to see if this is a good solution for your piano. I am a registered technician for Dampp Chaser, and thoroughly believe in the product’s value."
                                v-bind:image="piano3"
                            />
                        </div>
                    </div>
                </div>
                <div class="lg:flex">
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card
                                title="Rebuild or Restoration"
                                desc="I have experience repinning a number of pianos, giving new life to an old piano that cannot hold it’s tune anymore. And with this, the options come of how far would you like your repairs to go? I can restring pianos, hammers can be reshaped and replaced, to give a new brilliance to your piano. We can regulate the touch, to make your piano your own. Or your Great Grandmother’s piano sound brand new."
                                v-bind:image="piano2"
                            />
                        </div>
                    </div>
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card
                                title="String Replacement"
                                desc="Piano string replacement: Sometimes an old string lets go. It happens, especially in older pianos. These can be replaced! I have a full stock of piano strings, and can replace strings broken from play, or even if they let go during tuning. This takes time, and so is a flat rate per string. Bass strings can be replaced with universal strings, making your piano sound full again, and brighter. 
I can also do a full string replacement, which will require an estimate and at least a couple weeks of your piano in my shop. I do not move pianos, so pick up and drop off would be up to the customer."
                                v-bind:image="piano"
                            />
                        </div>
                    </div>
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card
                                title="Grand Piano Regulation"
                                desc="Grand Piano regulation takes two to three days, after which, your piano will be fine tuned with the touch, after touch, and smoothness of playing that you expect from a grand piano. It is a little less time to regulate an upright, so there will be an estimate on both types of pianos, and a block of at least two days to regulate them."
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
                                desc="Some of the work I love to do is set up your guitars, banjos, stringed instruments! I can fix your broken instruments, or we can drop the action, and give your instrument a new touch. Making it easier to play, and improve the tone, and volume."
                                v-bind:image="guitar"
                            />
                        </div>
                    </div>
                    <div class="mb-6 lg:mb-0 lg:w-1/3">
                        <div class="px-3">
                            <Card
                                title="Instrument Repair"
                                desc="Is your instrument broken, in disrepair, or in general need of some TLC? I can definitely fix your broken instruments, and return them to their former glory."
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
                    <p>
                        Please send us a message using our
                        <nuxt-link class="text-white" to="/contact"
                            ><span class="text-white font-bold"
                                >contact form.</span
                            ></nuxt-link
                        >
                    </p>
                </div>
            </Container>
        </ContentBackground>
    </div>
</template>

<script>
import piano from "~/assets/images/piano.jpg";
import piano2 from "~/assets/images/piano3.jpg";
import piano3 from "~/assets/images/keys.jpg";
import guitar from "~/assets/images/guitar.jpg";

export default {
    data() {
        return {
            piano,
            piano2,
            piano3,
            guitar
        };
    }
};
</script>
