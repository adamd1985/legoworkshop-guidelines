<template>
  <div id="home" class="white-box">
    <section id="hero" dark class="mx-0 px-0">
      <div>
        <v-parallax dark :src="bgHeroUrl" max-height="1024px" class="mb-10 pb-4">
          <v-row align="center" justify="center">
            <v-col cols="10">
              <v-row align="center" justify="center">
                <v-col cols="12" md="6" xl="8">
                  <div class=" mt-md-16 pt-md-16 mt-6 pt-6" style="text-shadow: 1px 1px 2px #131316 ;">
                    <div
                      class="text-md-h1 text-h4 font-weight-black transition-swing text-left banner lego-font"
                    >
                      Agile
                    </div>
                    <div
                      class="text-md-h1 text-h4 font-weight-black transition-swing text-left banner"
                    >
                      Development
                    </div>
                    <div
                      class="text-md-h1 text-h4 font-weight-black transition-swing text-left banner"
                    >
                      Workshop
                    </div>
                    <div
                      style="z-index: 10;"
                      class="text-md-h2 text-h5 font-weight-black transition-swing text-left mt-md-10 mt-4 mb-6 banner"
                    >
                      With Lego®!
                    </div>
                  </div>
                </v-col>
                <v-col cols="12" md="6" xl="4" class="hidden-sm-and-down" />
              </v-row>
            </v-col>
          </v-row>

          <div class="svg-border-waves mx-0 px-0">
            <img src="~/assets/img/wave2.svg">
          </div>
        </v-parallax>
      </div>
    </section>
    <section id="features" class=" ">
      <div class="py-12" />

      <v-container class="text-center mt-0 pt-0">
        <div class="text-md-h4 text-h5 font-weight-bold mb-3">
          An Agile Development Training
        </div>
        <div class="text-md-h6 text-h7 font-weight-bold mb-3">
          <v-icon dark color="#FFE330">
            mdi-toy-brick-marker
          </v-icon> 21st September 11-12:30pm - Room 4.01
        </div>

        <v-responsive class="mx-auto mb-md-12 mb-5 mt-md-12 mt-5" width="70vw">
          <v-divider class="mb-1" />
        </v-responsive>

        <v-row align="center" justify="center">
          <v-col
            cols="12"
            md="6"
          >
            <v-form ref="form" method="POST" class="contact-form">
              <v-responsive
                class="mx-auto mb-8 text-body-1"
                max-width="620"
              >
                Coaching Agile Development, in a simulation with Lego® gamification, is a modern method for experiencing <b>capacity planning</b>,
                <b>iterative execution</b>, and <b>self-organization principles</b> within a squad of professionals.
                <br><br>
                All are encouraged to join, a good squad is a mix of engineering,
                sales, graphics, business and product.
                The challenge in this training is to build the best city possible with Lego® building blocks, that meets the requirements of the "Product Owner”, within a set of restrictions.
              </v-responsive>
              <v-responsive
                class="mx-auto mb-8 text-body-1"
                max-width="620"
              >
                This culture and work principles drive our organization today.
              </v-responsive>
              <v-responsive
                class="mx-auto mb-8 text-body-1"
                max-width="620"
              >
                The workshop is set for up to 20 participants and has a run time of 1hour and 30 minutes max.
              </v-responsive>

              <v-responsive>
                <div class="py-12" />
                <a href="#contact" style="text-decoration: none; color: inherit;">
                  <v-btn
                    color="#FFE330"
                    fab
                    outlined
                  >
                    <v-icon dark>mdi-chevron-double-down</v-icon> <div class="font-weight-bold ml-3">register</div>
                  </v-btn>
                </a>
                <div class="py-12" />
              </v-responsive>
            </v-form>
          </v-col>
          <v-col
            cols="12"
            md="6"
          >
            <v-img :src="scrumUrl" class="rounded-lg mb-12" height="50vh" />
          </v-col>
        </v-row>

        <div v-if="$vuetify.display.name !== 'xs' && $vuetify.display.name !== 'sm'" class="py-12" />
        <div v-if="$vuetify.display.name !== 'xs' && $vuetify.display.name !== 'sm'" class="py-12" />
        <div v-if="$vuetify.display.name !== 'xs' && $vuetify.display.name !== 'sm'" class="py-12" />

        <div class="svg-border-waves mx-0 px-0">
          <img src="~/assets/img/wave.svg">
        </div>
      </v-container>
    </section>
  </div>
</template>

<script>
import bgHeroImage from '~/assets/img/bgHero.png'
import scrumImage from '~/assets/img/scrum.png'

export default {
  data: () => ({
    bgHeroUrl: bgHeroImage,
    scrumUrl: scrumImage
  })
}
</script>

<style scoped>
.banner{
  color: #FFE330;
}
</style>
