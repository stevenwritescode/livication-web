<template>
  <div>
    <template>
      <v-parallax
        dark
        src="@/assets/space-paint.jpg"
        height="300"
      >
        <v-row align="center" justify="center">
          <v-col class="text-center">
            <v-img
              :src="require('@/assets/Livication_Logo_Light.svg')"
              contain
              max-height="100"
            />
          </v-col>
        </v-row>
      </v-parallax>
    </template>
    <v-sheet elevation="2" max-width="960" class="mx-auto">
      <v-container>
        <v-row class="text-center">
          <v-col cols="12"> </v-col>

          <v-col class="mb-4">
            <h1 class="display-2 font-weight-bold mb-3">WHAT IS LIVICATION</h1>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h1 class="headline font-weight-bold mb-3">DEFINITION</h1>

            <p class="subheading font-weight-regular text-center">
              <strong>Livication</strong> is a blend of the words
              <em>living</em> and <em>dedication</em>, as if the latter began
              with the wrong word.
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h1 class="headline font-weight-bold mb-3">MISSION</h1>
            <p class="subheading font-weight-regular text-center">
              Who ever said <em>technology</em> had to be so <em>technical?</em
              ><br />
              Livication combines the creative arts with technology and
              engineering<br />
              to create innovative experiences for businesses of all sizes.<br />
            </p>
            <p class="subheading font-weight-regular text-center">
              Physically located on the Space Coast of Florida, we live among
              those who aim for the stars.<br />
              Digitally located within the Metaverse, we embrace experiences
              that can bring distant worlds together.
            </p>
          </v-col>

          <v-col class="mb-5 text-center" cols="12">
            <h1 class="display-2 font-weight-bold mb-3">SERVICES</h1>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <v-img
              :src="require('@/assets/blockchain.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
            />
            <h2 class="headline font-weight-bold mb-3">
              BLOCKCHAIN CONSULTING &amp; DEVELOPMENT
            </h2>
            <p class="subheading font-weight-regular text-center">
              First we <em>read</em> the internet, then we <em>wrote</em> the
              internet, now we <em>own</em> the internet.
            </p>
            <p class="subheading font-weight-regular text-center">
              Let Livication bring your business into the new Internet age.<br />
              We understand the potential that Web3 technologies have to put
              power into the hands of individuals.<br />
              Find out how your business can benefit from blockchain, smart
              contracts, non-fungible tokens, and decentralized currencies.
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h2 class="headline font-weight-bold mb-3">
              CRYPTOCURRENCY MINING
            </h2>
            <v-img
              :src="require('@/assets/mining.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
              position="top"
            />
            <p class="subheading font-weight-regular text-center">
              Make passive income supporting networks that support a more
              decentralized world.
            </p>
            <p class="subheading font-weight-regular text-center">
              Livication can help get you started with cryptocurrency mining by
              sourcing equipment,<br />
              planning or building your mining farm, reducing your electric bill
              with renewable energy sources,<br />
              and optimizing your build for maximum efficiency, safety, and
              maintainability.
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h2 class="headline font-weight-bold mb-3">
              METAVERSE DEVELOPMENT
            </h2>
            <v-img
              :src="require('@/assets/metaverse.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
              position="top"
            />
            <p class="subheading font-weight-regular text-center">
              Bring your business into a world of 24/7 worldwide advertisement!
            </p>
            <p class="subheading font-weight-regular text-center">
              Livication owns virtual land in the Decentraland Metaverse that
              can be used to garner<br />
              worldwide recognition for your brand. Benefit from a world that is
              less saturated with advertisements,<br />
              and speak to an audience that is eager for new experiences.<br />
              Build a home for your business that is unbound by the limitations
              of the physical world.<br />
              Today a floating island, tomorrow a skyscraper, the next day a
              festival stage.<br />
              Keep your audience wondering what you'll do next!
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h2 class="headline font-weight-bold mb-3">
              SOFTWARE PRODUCT PLANNING &amp; DEVELOPMENT
            </h2>
            <v-img
              :src="require('@/assets/software.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
            />
            <p class="subheading font-weight-regular text-center">
              Build that thing that nobody has thought of yet!
            </p>
            <p class="subheading font-weight-regular text-center">
              Plan the architecture of your software project, determine a scope
              and budget, <br />and hire qualified software engineers that can
              bring your vision to life.<br />
              Smaller projects can be built in-house by Livication!
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h2 class="headline font-weight-bold mb-3">
              LIVE VIDEO PRODUCTION
            </h2>
            <v-img
              :src="require('@/assets/video.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
            />
            <p class="subheading font-weight-regular text-center">
              Put away the shaky cell phone feed and take your live stream to
              the next level!
            </p>
            <p class="subheading font-weight-regular text-center">
              We can stream your event, performance, or seminar with
              professional-quality broadcasting equipment.<br />
              Switch between multiple cameras, add virtual backgrounds, wire in
              professionally mixed audio, and more.<br />
              Show your innovative side and stream your live event from our land
              in the Metaverse!
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h2 class="headline font-weight-bold mb-3">AUDIO ENGINEERING</h2>
            <v-img
              :src="require('@/assets/audio-board.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
              position="center"
            />
            <p class="subheading font-weight-regular text-center">
              Make your business heard!
            </p>
            <p class="subheading font-weight-regular text-center">
              Provide a compelling aural experience for your product with
              Livication's audio engineering services.<br />
              Our in-house studio can provide sound design, music production,
              voice-over recording, podcast production, and more.<br />
              Have a live event coming up that needs to sound amazing?
              Livication can provide on-site live sound engineering.
            </p>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>
            <h2 class="headline font-weight-bold mb-3">CUSTOM AUTOMATION</h2>
            <v-img
              :src="require('@/assets/automation.jpg')"
              class="mx-auto my-3"
              height="150"
              width="60%"
            />
            <p class="subheading font-weight-regular text-center">
              Leave the menial, tedious tasks to the robots. Save your time and
              sanity with automation!
            </p>
            <p class="subheading font-weight-regular text-center">
              Let your aquarium change its own water.<br />
              Have your doors lock themselves when you go to bed.<br />
              Never worry again about whether you forgot to close the garage.<br />
              We can recommend automation solutions for your home or business<br />
              and help you program them to compliment your busy schedule.
            </p>
          </v-col>
          <v-col class="mb-5" cols="12">
            <h1 class="display-2 font-weight-bold mb-3">GET STARTED</h1>
            <v-divider width="200" class="mx-auto mb-3"></v-divider>

            <h2 class="headline font-weight-bold mb-3">
              CONTACT US TODAY
            </h2>
            <p class="subheading font-weight-regular text-center">
              <strong>Email:</strong> info@livication.com<br />
              <strong>Phone/Text Message:</strong> 303-775-7933 (Supports
              iMessage)<br />
              <a href="https://discord.gg/sjtNgQvJAU"
                ><strong>Click To Join Our Discord Server</strong></a
              >
            </p>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Home',

  data: () => ({})
})
</script>
