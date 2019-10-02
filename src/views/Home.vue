<template>
  <div class="home">
     
    <v-container class="form">
          <v-row align="center" justify="center">
                    <v-img class="image"
                      :src="require('../assets/app.png')"
                      aspect-ratio="1"
                      
                      max-width="100"
                      max-height="100"
                    ></v-img>
          </v-row>
          <v-container>
            <v-layout row wrap>
              <v-flex xs10>
                <v-btn rounded color="#F8D430" width="180px">
                  Current Order
                </v-btn>
              </v-flex>

               <v-flex xs2>
                <v-btn class="mx-2" fab dark small width="36px" height="36px" color="#B71C1C">
                  <v-icon dark>mdi-delete</v-icon>
                </v-btn> 
              </v-flex>
            </v-layout>
          </v-container>
          <!--<v-container>
          <v-column>
              <v-btn rounded color="#F8D430" width="180px">
                Current Order
              </v-btn>
          </v-column>

          <v-column >
            <v-btn class="mx-2" fab dark small color="#B71C1C">
              <v-icon dark>mdi-delete</v-icon>
            </v-btn>
          </v-column>
          </v-container>-->
        
    </v-container>

    <v-container>
      <v-layout row wrap>
        <v-flex xs12>
          <v-card >
            <!--<v-carousel>-->
              <v-container>
                <v-layout row>
                  <v-flex xs12 >
                    
                      <v-carousel height="200px">
                      <v-row align="center" justify="center">  
                      <v-img
                        
                        :src="require('../assets/app2.png')"
                        class="white--text"
                        height="200px"
                       
                        max-width="340"
                        max-height="340"
                      >
                      
                        <v-card-title
                          class="fill-height align-end"
                          
                        ></v-card-title>
                      </v-img>
                      </v-row>
                      </v-carousel>
                    
                        <v-row align="center" justify="center">
                        <v-card-actions >
                          <div class="flex-grow-1"></div>

                          <v-btn rounded color="#F8D430" width="180px">
                            Book
                          </v-btn>

                        </v-card-actions>
                        </v-row>
                    
                  </v-flex>
                </v-layout>
              </v-container>
            <!--</v-carousel>-->
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>

    <v-container>
      <v-layout row wrap>
        <v-flex xs12>
          <!--<v-card>-->
            <!--<v-container>-->
              <v-layout row>
                <v-flex xs12>
                  <v-tabs
                       color="#F8D430"
                      v-model="tab"
                      background-color="#1E1F28"
                      centered
                      dark
                      icons-and-text
                    >
                      <v-tabs-slider></v-tabs-slider>

                      <v-tab href="#tab-1">
                        Home
                        <v-icon>mdi-home</v-icon>
                      </v-tab>

                      <v-tab href="#tab-2">
                        History
                        <v-icon>mdi-history</v-icon>
                      </v-tab>

                      <v-tab href="#tab-3">
                       Inbox
                        <v-icon>mdi-inbox</v-icon>
                      </v-tab>

                      <v-tab href="#tab-4">
                        Profile
                        <v-icon>mdi-account-box</v-icon>
                      </v-tab>
                    </v-tabs>

                    <v-tabs-items v-model="tab">
                      <v-tab-item
                        v-for="i in 4"
                        :key="i"
                        :value="'tab-' + i"
                      >
                      </v-tab-item>
                    </v-tabs-items>
                </v-flex>
              </v-layout>
            <!--</v-container>-->
          <!--</v-card>-->
        </v-flex>
      </v-layout> 
      </v-layout>
    </v-container>

        <!--<v-card>
          <v-tabs
            v-model="tab"
            background-color="#1E1F28"
            centered
            dark
            icons-and-text
          >
            <v-tabs-slider></v-tabs-slider>

            <v-tab href="#tab-1">
              Recents
              <v-icon>mdi-phone</v-icon>
            </v-tab>

            <v-tab href="#tab-2">
              Recents
              <v-icon>mdi-phone</v-icon>
            </v-tab>

            <v-tab href="#tab-3">
              Favorites
              <v-icon>mdi-heart</v-icon>
            </v-tab>

            <v-tab href="#tab-4">
              Nearby
              <v-icon>mdi-account-box</v-icon>
            </v-tab>
          </v-tabs>

          <v-tabs-items v-model="tab">
            <v-tab-item
              v-for="i in 4"
              :key="i"
              :value="'tab-' + i"
            >
            </v-tab-item>
          </v-tabs-items>
        </v-card>-->

    </div>
</template>

<script>


export default {
  components: {
  
  },
   data: () => ({
      cards: [
        { title: 'Pre-fab homes', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 12 },
        { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 6 },
        { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 6 },
      ],
      items:[
        {
          src: '../assets/app2.png'
        }
      ]
    }),
    methods:{

    }
};
</script>

<style>
.form{
  /*height:50px;
  padding-top:100px;*/
  height:189px;
  background-color:#1E1F28;
}

.image{
  /*margin-top:-100px;*/
}

/*.home{
  margin-top:100px;
}*/
.btn{
  margin-left:510px;
}
/*.card{
  margin-left:100px;
  margin-top:100px;*/
/*}*/
</style>
