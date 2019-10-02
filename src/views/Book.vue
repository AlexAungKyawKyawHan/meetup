<template>
    <div class="book">
            <v-container>
      <v-layout row>
        <v-flex xs12 sm6 offset-sm3>
          <v-card>
            <v-card-text>
              <v-container>
                <form>
                  <v-layout row>
                    <v-flex xs12>
                        <v-select
                            :items="items"
                            label="Type"
                        ></v-select>
                    </v-flex>
                  </v-layout> 

                  <v-layout row>
                    <v-flex xs12>
                      <v-text-field name="password" label="Notes"></v-text-field>
                    </v-flex>
                  </v-layout> 

                  <v-layout row justify="center">
                      <v-flex xs12>
                          <v-date-picker v-model="picker"></v-date-picker>
                      </v-flex>
                  </v-layout>

                  <v-layout row >
                    <v-flex xs12>
                      <v-btn type="submit" dark color="pink" class="btn" to="/book">Book</v-btn>
                    </v-flex>
                  </v-layout>
                </form>
              </v-container>
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
    </div>
</template>

<script>
    export default{
        data: () => ({
      items: ['WM', 'AC', 'REF', 'CCTV'],
      picker:new Date().toISOString().substr(0, 10),
    }),
    }
</script>

<style>
.book{
  margin-top:0px;
}
.btn{
  margin-left:510px;
}
</style>    