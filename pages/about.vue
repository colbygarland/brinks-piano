<template>
  <div>
    <Content>
      <Container>
        <H1>About Brink's Piano Works</H1>
        <div class="prose">
          <div class="lg:flex">
            <div>
              <img :src="Steve" alt="Steve Vanden Brink" class="pr-6" />
            </div>
            <div class="lg:mt-10 xl:mt-20">
              <p>
                At Brink’s Piano works, I have a vision for instruments to work
                and sound their very best, and as such I have surrounded myself
                with two experienced Technicians.
              </p>
              <p>
                I have joined international forums, am taking two courses, and
                am apprenticing under Grande Prairie’s best guitar tech.
              </p>
              <p>
                One can never stop learning, and so this is my goal, to strive
                to excellence in all things relating to instruments, whether it
                is tuning a piano, or fixing a ukulele.
              </p>
              <p>
                I am a father, and husband, and I believe in passing on beauty,
                joy, and the sheer delight of music in all forms to the
                generations after my own. Investing in music is, to me, one of
                the most worthwhile things we can do. Because music is a
                language that all people speak, and understand. We make music,
                better.
              </p>
            </div>
          </div>
        </div>
      </Container>
    </Content>
  </div>
</template>

<script>
import Steve from "~/assets/images/Steve.jpg";
export default {
  data() {
    return {
      Steve,
    };
  },
};
</script>
