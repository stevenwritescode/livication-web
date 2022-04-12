<template>
  <div>
    <template>
      <v-parallax dark src="@/assets/space-paint.jpg" height="300">
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
        <v-row class="text-center mt-4">
          <v-col class="mb-4">
            <h1 class="display-2 font-weight-bold mb-4">
              {{ about.title }}
            </h1>
            <v-divider width="200" class="mx-auto mb-4"></v-divider>

            <p class="title font-weight-regular text-center mb-0"></p>
            <p
              v-html="about.definition"
              class="text-body-2 font-weight-regular text-center mt-0"
            ></p>

            <v-divider width="200" class="mx-auto mb-4"></v-divider>

            <div v-for="(section, i) in about.sections" :key="i">
              <v-lazy
                v-model="section.showing"
                :key="i"
                :options="{
                  threshold: 0.5
                }"
                class="text-center mx-auto"
                transition="fade-transition"
              >
                <h1 class="headline font-weight-bold mb-4">
                  {{ section.title }}
                </h1>
              </v-lazy>

              <div v-for="(paragraph, x) in section.paragraphs" :key="x">
                <v-lazy
                  v-model="section.showing"
                  :key="i"
                  :options="{
                    threshold: 0.5
                  }"
                  class="text-center mx-auto"
                  transition="fade-transition"
                >
                  <p
                    class="subheading font-weight-regular text-center"
                    v-html="paragraph"
                  ></p>
                </v-lazy>
              </div>
            </div>
          </v-col>
          <v-col class=" text-center" cols="12">
            <h1
              class="display-2 font-weight-bold mb-4"
              v-html="services.title"
            ></h1>
            <div v-for="(section, i) in services.sections" :key="i">
              <v-lazy
                :options="{
                  threshold: 0.5
                }"
                class="text-center mx-auto"
                transition="fade-transition"
              >
                <section>
                  <h2
                    v-html="section.title"
                    class="headline font-weight-bold mb-4"
                  ></h2>
                  <v-divider width="200" class="mx-auto mb-4"></v-divider>
                </section>
              </v-lazy>
              <v-lazy
                :options="{
                  threshold: 0.5
                }"
                class="text-center mx-auto"
                transition="fade-transition"
              >
                <section>
                  <v-img
                    :src="section.imagePath"
                    class="mx-auto my-3"
                    height="150"
                    width="60%"
                  />
                  <div v-for="(paragraph, p) in section.paragraphs" :key="p" class="paragraph mx-auto">
                    <p
                      v-html="paragraph"
                      class="subheading font-weight-regular text-center d-inline-block"
                    ></p>
                  </div>
                  <v-divider
                    v-if="i < services.sections.length - 1"
                    width="200"
                    class="mx-auto mb-4"
                  ></v-divider>
                </section>
              </v-lazy>
            </div>
          </v-col>
          <v-col class="mb-6" cols="12">
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

  data: () => ({
    about: {
      title: 'LIV[ING] [DED]ICATION',
      definition:
        '<strong>Livication</strong> is a blend of the words <em>living</em> and <em>dedication.</em>',
      sections: [
        {
          title: 'MISSION',
          paragraphs: [
            'Who ever said <em>technology</em> had to be so <em>technical?</em><br /> Livication combines the creative arts with technology and engineering<br /> to create innovative experiences for businesses of all sizes.',
            'Physically located on the Space Coast of Florida, we live among those who aim for the stars.<br /> Digitally located within the Metaverse, we embrace distant friends and diverse experiences.'
          ],
          showing: false
        }
      ]
    },
    services: {
      title: 'SERVICES',
      sections: [
        {
          title: 'BLOCKCHAIN CONSULTING &amp; DEVELOPMENT',
          imagePath: `${require('@/assets/blockchain.jpg')}`,
          paragraphs: [
            'First we <em>read</em> the internet, then we <em>wrote</em> the internet, now we <em>own</em> the internet.',
            'Let Livication bring your business into the new Internet age.<br /> We understand the potential that Web3 technologies have to put power into the hands of individuals.<br /> Find out how your business can benefit from blockchain, smart contracts, non-fungible tokens, and decentralized currencies.'
          ]
        },
        {
          title: 'CRYPTOCURRENCY MINING',
          imagePath: `${require('@/assets/mining.jpg')}`,
          paragraphs: [
            'Make passive income supporting networks that support a more decentralized world.',
            'Livication can help get you started with cryptocurrency mining by sourcing equipment, planning or building your mining farm, reducing your electric bill with renewable energy sources, and optimizing your build for maximum efficiency, safety, and maintainability.'
          ]
        },
        {
          title: 'METAVERSE DEVELOPMENT',
          imagePath: `${require('@/assets/metaverse.jpg')}`,
          paragraphs: [
            'Bring your business into a world of 24/7 worldwide advertisement!',
            `Rent or buy land in the Metaverse and garner worldwide recognition for your brand for 24 hours a day.<br /> Benefit from a world that is less saturated with advertisements, and find an audience that is eager for new experiences.<br /> Build a home for your business that is unbound by the limitations of the physical world.<br /> Today a floating island, tomorrow a skyscraper, the next day a festival stage.<br /> Keep your audience wondering what you'll do next!`
          ]
        },
        {
          title: 'SOFTWARE PRODUCT PLANNING &amp; DEVELOPMENT',
          imagePath: `${require('@/assets/software.jpg')}`,
          paragraphs: [
            'Build that thing that nobody has thought of yet!',
            'Plan the architecture of your software project, determine a scope and budget, <br />and hire qualified software engineers that can bring your vision to life.<br /> Some projects can be built in-house by Livication!'
          ]
        },
        {
          title: 'LIVE VIDEO PRODUCTION',
          imagePath: `${require('@/assets/video.jpg')}`,
          paragraphs: [
            'Put away the shaky cell phone feed and take your live stream to the next level!',
            'We can stream your event, performance, or seminar with professional-quality broadcasting equipment.<br /> Switch between multiple cameras, add virtual backgrounds, wire in professionally mixed audio, and more.<br /> Show your innovative side and stream your live event from our land in the Metaverse!'
          ]
        },
        {
          title: 'AUDIO ENGINEERING',
          imagePath: `${require('@/assets/audio-board.jpg')}`,
          paragraphs: [
            'Make your business heard!',
            `Provide a compelling aural experience for your product with Livication's audio engineering services.<br /> Our in-house studio can provide sound design, music production, voice-over recording, podcast production, and more.<br /> Have a live event coming up that needs to sound amazing? Livication can provide on-site live sound engineering.`
          ]
        },
        {
          title: 'CUSTOM AUTOMATION',
          imagePath: `${require('@/assets/automation.jpg')}`,
          paragraphs: [
            'Leave the menial, tedious tasks to the robots. Save your time and sanity with automation!',
            `Let your aquarium change its own water.<br /> Have your doors lock themselves when you go to bed.<br /> Never worry again about whether you forgot to close the garage.<br /> We can recommend automation solutions for your home or business<br /> and help you program them to compliment your busy schedule.`
          ]
        }
      ]
    }
  })
})
</script>

<style scoped>
.paragraph {
  max-width: 850px
}
</style>