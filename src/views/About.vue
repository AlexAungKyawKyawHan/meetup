<template>
      <v-container class="about">
      <v-layout row>
        <v-flex xs12 sm6 offset-sm3>
          <v-card>
            <v-card-text>
              <v-container>
                <form>
                  <v-layout row>
                    <v-flex xs12>
                      <v-text-field name="username" label="UserName"></v-text-field>
                    </v-flex>
                  </v-layout> 

                  <v-layout row>
                    <v-flex xs12>
                      <v-text-field name="password" label="Password" type="password"></v-text-field>
                    </v-flex>
                  </v-layout> 

                  <v-layout row>
                    <v-flex xs12>
                      <v-text-field name="Confirmpassword" label="ConfirmPassword" type="password"></v-text-field>
                    </v-flex>
                  </v-layout> 

                  <v-layout row>
                    <v-flex xs12>
                      <v-btn type="submit" dark color="pink" class="btn" to="book">Sign Up</v-btn>
                    </v-flex>
                  </v-layout>
                </form>
              </v-container>
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
</template>

<script>
  export default{

  }
</script>

<style>
  .about{
  margin-top:100px;
}
.btn{
  margin-left:510px;
}
</style>