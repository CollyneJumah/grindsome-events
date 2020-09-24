<template>
  <Layout>

    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
    <!-- <g-image alt="Example image" src="~/favicon.png" width="135" /> -->
    <v-container>
      <v-row>
        <v-col sm="6" offset-sm="4">
          <v-tabs v-model="tab" grow>
            <v-tab>Item One</v-tab>
              <v-tab>Item Two</v-tab>
              <v-tab>Item Three</v-tab>
            </v-tabs>
              <v-card class="mx-auto" max-width="400">
                <iframe class="white--text align-end" width="400" height="200px" src="https://www.youtube.com/embed/wBTnD_ob12M" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>
                <v-card-text class="text--primary">
                  <div>Whitehaven Beach</div>

                  <div>Whitsunday Island, Whitsunday Islands</div>
                </v-card-text>

                <v-card-actions>
                  <v-btn
                    color="orange"
                    text
                  >
                    Share
                  </v-btn>

                  <v-btn
                    color="orange"
                    text
                  >
                    Explore
                  </v-btn>
                </v-card-actions>
              </v-card>
              <v-card class="mx-auto" max-width="400">
                <iframe class="white--text align-end" width="400" height="200px" src="https://www.youtube.com/embed/wBTnD_ob12M" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>
                <v-card-text class="text--primary">
                  <div>Whitehaven Beach</div>

                  <div>Whitsunday Island, Whitsunday Islands</div>
                </v-card-text>

                <v-card-actions>
                  <v-btn
                    color="orange"
                    text
                  >
                    Share
                  </v-btn>

                  <v-btn
                    color="orange"
                    text
                  >
                    Explore
                  </v-btn>
                </v-card-actions>
              </v-card>
              <v-card class="mx-auto" max-width="400">
                <iframe class="white--text align-end" width="400" height="200px" src="https://www.youtube.com/embed/wBTnD_ob12M" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>
                <v-card-text class="text--primary">
                  <div>Whitehaven Beach</div>

                  <div>Whitsunday Island, Whitsunday Islands</div>
                </v-card-text>

                <v-card-actions>
                  <v-btn
                    color="orange"
                    text
                  >
                    Share
                  </v-btn>

                  <v-btn
                    color="orange"
                    text
                  >
                    Explore
                  </v-btn>
                </v-card-actions>
              </v-card>
        </v-col>
      </v-row>
    </v-container>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  data(){
    return {
      tab: 0
    }
  },
  watch:{
      tab(val)
      {
        if(this.tab === 0)
        {
          this.showAllEvents()
        }else{
          this.showEventsByType()
        }
      }
    },
  methods:{
    showAllEvents(){
      console.log('All')
    },
    showEventsByType()
    {
      console.log('Event Types')
    }
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
