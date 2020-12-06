<template>
  <div>
    <div class="width-1920">
      <header class="header">
        <b-container fluid>
          <b-row>
            <b-col cols="12" md="9">
              <h1>Bringing together <br> the smartest people</h1>
              <p class="mt-4">
                We believe when true winners win the game, there will be potential projects to invest.
                There is when the magic happens. The result is better country to live in and authentic
                selves to work with.
              </p>
              <b-input-group class="mt-4">
                <b-form-input placeholder="Please type here..."></b-form-input>
                <b-input-group-append>
                  <b-button variant="success" class="px-4" @click="$router.push('/search')">Search</b-button>
                </b-input-group-append>
              </b-input-group>
            </b-col>
            <b-col cols="12" md="3"></b-col>
          </b-row>
        </b-container>
      </header>
    </div>
    <div class="principles">
      <section class="section">
        <b-container fluid>
          <b-row>
            <b-col cols="12">
              <h1>Our Principles</h1>
            </b-col>
            <b-col cols="12" md="6" v-for="i of items" :key="i.id">
              <TheCard style="margin-bottom: 70px" :item="i" />
            </b-col>
          </b-row>
        </b-container>
      </section>
    </div>
    <div class="motto">
      <section class="section">
        <h1 class="text-center">Be your better self</h1>
        <p class="text-center">Are you attending a competition or searching for potential projects worth investing? Then held-in.uz is the source you need. Here you can find about competitions and the projects in Uzbekistan</p>
        <p class="text-center"><nuxt-link to="/">See Competitions</nuxt-link></p>
      </section>
    </div>
  </div>
</template>

<script>
import TheCard from "@/components/TheCard";

export default {
  components: {
    TheCard
  },
  data() {
    return {
      items: [
        { id: 1, title: 'Follow the data', description: 'Teams with potential projects - will have a greater impact. By analysing data about competitions and contests from mass media we answer questions "Why, when & where to invest".' },
        { id: 2, title: 'Be proactive', description: 'While talent and potential are equally distributed, opportunity is not. There\'s always more we can do to build better community. Everyone has access to better understanding of a competitions being held.' },
        { id: 3, title: 'Keep improving', description: 'We publish all the competition events to achieve continuous improvement. Navigate uncertainity in a rapidly changing market and identify growth opportunities for top and bottom line.' },
        { id: 4, title: 'Invest in smart people', description: 'Unlock new ideas and growth by unleashing the power and creativity of your own organisation and people. Solve key business challenges by engaging with the world\'s most innovative startups.' },
      ] 
    }
  }
}
</script>