<template>
    <div class="container-fluid contact">
      <br><br>
      <div class="container">
                        <div class="offset-md-1 col-md-10 ">
                           <div class="row">
                              <div class="col-md-7 col-sm-12">
                                 <div class="tunapic">
                                    <img alt="Vue logo" src="../assets/Mask Group 13.jpg">
                                 </div>
                              </div>
                           

                              <div class="col-md-4 col-sm-12">
                                 <p class="tuna">TUNA</p>
                                  <p class="tunadetail">
                                   SOLID, CHUCK, FLAKE, SHREDDED
                                  </p>
                                    <br>
                                    <p class="detail">
                                    Pellentesque semper quis neque dictum hendrerit. Sed nulla ipsum, 
                                    porttitor pharetra tortor in,consequat imperdiet nisi. Phasellus at quam tristique, 
                                    cursus tellus vitae, convallis neque.
                                  </p>

                                 <hr color=#3b98c9>
                              
                              </div>
                           </div>
                        </div>
                        <v-row>
                          <p class="SPEICIES">SPEICIES</p>
                        </v-row>
                       
    <v-slide-group
      v-model="model"
      class="pa-4"
      active-class="success"
      show-arrows
    >
      <v-slide-item
        v-for="n in 6"
        :key="n"
        v-slot:default="{ active, toggle }"
      >
        <v-card
          :color="active ? undefined : 'white lighten-1'"
          class="ma-4"
          height="400"
          width="300"
          @click="toggle"
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
          <div class="fishpic">
                  <img alt="Vue logo" src="../assets/Image 76.png">
                  
            </div>
            <v-scale-transition>
            </v-scale-transition>
          </v-row>
        </v-card>
      </v-slide-item>
    </v-slide-group>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
      model: null,
    }),
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.tuna{
  font-family: Roboto;
  font-size: 30px;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
  text-align: left;
  color: #3b98c9;
}

.fishpic{
  margin: 130px 0px 0px;
}

.tunadetail {
  font-family: Roboto;
  font-size: 20px;
  font-weight: 300;
  font-stretch: normal;
  font-style: normal;
  text-align: left;
  color: #939393;
}

.detail{
  width: 353px;
  height: 113px;
  font-family: Roboto;
  font-size: 14px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.36;
  letter-spacing: normal;
  text-align: left;
  color: #a8a8a8;
}

h3 {
  margin: 40px 0 0;
}
.SPEICIES {
  width: 248px;
  height: 66px;
  font-family: Roboto;
  font-size: 50px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.6;
  letter-spacing: 5px;
  text-align: left;
  color: #ddc7a9;
  margin-left: 40px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
