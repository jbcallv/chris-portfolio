<template>
  <transition
    appear
    enter-active-class="animated fadeIn"
    leave-active-class="animated fadeOut"
  >
    <q-page class="flex flex-center">
      <div class="row full-width justify-center items-center">
        <div class="col-12 col-md-5 col-lg-4 col-xl-3 q-pr-xl q-pl-xl">
          <div class="text-h2 text-weight-light q-pb-lg gt-sm">About me</div>
          <div class="text-h3 text-center text-weight-light q-pb-lg lt-md">
            About me
          </div>

          <div class="text-h5 text-weight-light text-grey gt-sm q-pb-lg">
            I'm a Data Scientist. I have a passion for anything business
            analytics and have been working in the Data Science industry for
            {{ new Date().getFullYear() - 2023 }} years.
          </div>

          <div class="text-h5 text-weight-light text-grey gt-sm q-pb-lg">
            I'm originally from Jamestown, Virginia and have always loved the
            unique culture and atmosphere there. In my free time, you can find
            me talking with
            <q-btn
              no-caps
              color="#121212"
              label="Barbara"
              @click="openURL('https://www.linkedin.com/in/callbarbara/')"
            />
            or trying out new recipes in the kitchen.
          </div>

          <div
            class="text-h6 text-center text-weight-light text-grey lt-md q-pb-lg"
          >
            I'm a Data Scientist. I have a passion for anything business
            analytics and have been working in the Data Science industry for
            {{ new Date().getFullYear() - 2023 }} years.
          </div>

          <div
            class="text-h6 text-center text-weight-light text-grey lt-md q-pb-lg"
          >
            I'm originally from Jamestown, Virginia and have always loved the
            unique culture and atmosphere there. In my free time, you can find
            me talking with
            <q-btn
              no-caps
              color="#121212"
              label="Barbara"
              @click="openURL('https://www.linkedin.com/in/callbarbara/')"
            />
            or trying out new recipes in the kitchen.
          </div>
        </div>

        <div class="col-10 col-md-5 col-lg-4 col-xl-3">
          <div class="row q-gutter-sm q-pb-sm justify-center">
            <div
              class="col-12 col-md"
              style="aspect-ratio: 1/1; max-width: 500px"
            >
              <q-card class="full-height full-width bg-dark">
                <q-card-section>
                  <div class="text-h6 text-weight-bold text-center">
                    Languages
                  </div>
                </q-card-section>

                <q-separator inset color="accent" size="3px" />

                <q-card-section>
                  <q-item class="text-body1">English, Portugese</q-item>
                  <q-item class="text-body1">Python, R</q-item>
                </q-card-section>
              </q-card>
            </div>

            <div
              class="col-12 col-md"
              style="aspect-ratio: 1/1; max-width: 500px"
            >
              <q-card class="full-height full-width bg-dark">
                <q-card-section
                  ><div class="text-h6 text-weight-bold text-center">
                    Frameworks
                  </div>
                </q-card-section>

                <q-separator inset color="accent" size="3px" />

                <q-card-section>
                  <q-item class="text-body1">React.js, Next.js, MUI</q-item>
                  <q-item class="text-body1">Vue.js, Quasar</q-item>
                  <q-item class="text-body1">Node.js, Express.js </q-item>
                </q-card-section>
              </q-card>
            </div>
          </div>

          <div class="row q-gutter-sm justify-center">
            <div
              class="col-12 col-md"
              style="aspect-ratio: 1/1; max-width: 500px"
            >
              <q-card class="full-height full-width bg-dark">
                <q-card-section>
                  <div class="text-h6 text-weight-bold text-center">
                    Databases
                  </div>
                </q-card-section>

                <q-separator inset color="accent" size="3px" />

                <q-card-section>
                  <q-item class="text-body1">PostgreSQL, Psycopg2</q-item>
                  <q-item class="text-body1">MongoDB, Prisma ORM</q-item>
                </q-card-section>
              </q-card>
            </div>

            <div
              class="col-12 col-md"
              style="aspect-ratio: 1/1; max-width: 500px"
            >
              <q-card class="full-height full-width bg-dark">
                <q-card-section>
                  <div class="text-h6 text-weight-bold text-center">Tools</div>
                </q-card-section>

                <q-separator inset color="accent" size="3px" />

                <q-card-section>
                  <q-item class="text-body1"
                    >Jira, Confluence, Bitbucket</q-item
                  >
                  <q-item class="text-body1"> Netlify, DigitalOcean</q-item>
                  <q-item class="text-body1">Vim, VSCode, Git</q-item>
                </q-card-section>
              </q-card>
            </div>
          </div>
        </div>
      </div>
    </q-page>
  </transition>
</template>

<script>
import { openURL } from "quasar";

export default {
  name: "AboutPage",

  setup() {
    return { openURL };
  },
};
</script>
