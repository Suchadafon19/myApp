<template>
    <div class="container-fluid contact">
      <br><br>
          <div class="offset-md-1 col-md-9 ">
              <div class="row">
                  <div class="col-md-8 col-sm-12">
                        <div class="tunapic">
                            <img alt="tunapic" src="../assets/Mask Group 13.jpg">
                        </div>
                  </div>
                           
               <div class="col-md-4 col-sm-12">
                  <p class="tuna">TUNA</p>
                    <p class="tunadetail">
                        SOLID, CHUCK, FLAKE, SHREDDED
                    </p><br>
                    <p class="detail">
                        Pellentesque semper quis neque dictum hendrerit. Sed nulla ipsum, 
                        porttitor pharetra tortor in,consequat imperdiet nisi. Phasellus at quam tristique, 
                        cursus tellus vitae, convallis neque.
                    </p>
                    <hr color=#3b98c9>          
                </div>
              </div>
          </div><br>
                        <v-content>
                          <v-row>
                            <p class="SPEICIES">SPEICIES</p>
                          </v-row>
                        </v-content>
      <div class="container">
        <v-row class="fill-height" align="center" justify="center">
            <template v-for="(item, i) in items">
                <v-col :key="i">
                        <v-row align="center" justify="center">
                            <v-col cols="12">
                              <v-row>
                              <v-hover
                                v-slot:default="{ hover }"
                              >
                                <v-card
                                  :elevation="hover ? 8 : 2"
                                  class="slide"
                                  height="400"
                                  width="300"
                                >
                                  <v-card-text class="title orange--text">
                                      {{ item.title }}
                                  </v-card-text>

                                  <p class="text">
                                      {{ item.text }}
                                  </p>

                                  <div class="fishpic">
                                      <v-img :src="item.img"></v-img>
                                  </div>
                                </v-card>
                              </v-hover>
                              </v-row>
                            </v-col>
                        </v-row>
                </v-col>
          </template>
        </v-row>
      </div>
      <br>
  <v-content>
      <v-row>
            <p class="SPEICIES">MEAT</p>
      </v-row>
  </v-content>
<v-container>
      <v-row justify="space-between">
    <v-card flat>
        <v-card-title>
        
            <v-row>
            
             <v-col cols="11" md="2" class="mx-9">
                <h6 class="meatfont">SOLID</h6>
                <img alt="tunapic" src="../assets/Group 201.png">
              </v-col>

              <v-col cols="11" md="2" class="mx-9">
                <h6 class="meatfont">CHUCK</h6>
                <img alt="tunapic" src="../assets/Group 203.png">
              </v-col>

              <v-col cols="11" md="2" class="mx-9">
                <h6 class="meatfont">FLAKE</h6>
                <img alt="tunapic" src="../assets/Group 202.png">
             </v-col>

             <v-col cols="11" md="2" class="mx-9">
                <h6 class="meatfont">SHREDDED</h6>
                <img alt="tunapic" src="../assets/Group 198.png">
             </v-col>
             
            </v-row>
            
        </v-card-title>
      </v-card>
      </v-row>
</v-container>

      <v-card
        class="mx-auto"
        color=#f9c410
      >
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title class="media">MEDIA</v-list-item-title>
              <v-list-item-subtitle></v-list-item-subtitle>
            </v-list-item-content>
          </v-list-item>
  
            <v-container>
              <v-card>
              <v-row justify="space-between">
                <v-col
                  cols="auto">
                  <v-row>
                    <v-row>
                    
                    
                    <v-col cols="10" md="2" class="mx-9">
                        <h6 class="font">BRINE</h6>
                        <div class="pic">
                        <img alt="tunapic" src="../assets/Image 92.png">
                        </div>
                      </v-col>
                  

                      <v-col cols="10" md="2" class="mx-9">
                        <h6 class="font">CHUCK</h6>
                        <img alt="tunapic" src="../assets/Image 68.png">
                      </v-col>

                      <v-col cols="10" md="2" class="mx-9">
                        <h6 class="font">FLAKE</h6>
                        <img alt="tunapic" src="../assets/Image 91.png">
                    </v-col>

                    <v-col cols="10" md="2" class="mx-9">
                        <h6 class="font">SHREDDED</h6>
                        <img alt="tunapic" src="../assets/Mask Group 20.jpg">
                    </v-col>
                    
                    </v-row>
                  </v-row>
                </v-col>
              </v-row>
              </v-card>
            </v-container>
  </v-card>
 
   <v-list-item>
      <v-list-item-content>
        <v-list-item-title class="size">SIZE</v-list-item-title>
        <v-list-item-subtitle></v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>
  
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
      icons: ['mdi-rewind', 'mdi-play', 'mdi-fast-forward'],
      items: [
        {
          title: 'ALBACORE',
          text: '(Thunnus alalunga)',
          img: 'https://www.img.in.th/images/18aeae2fcdeedb76cedcf3337e46a8d0.png',
        },
        {
          title: 'TONGOL',
          text: '(hunnus tonggol)',
          img: 'https://www.img.in.th/images/f9920ba652f3ebe60042fd990c60b2f8.png',
        },
        {
          title: 'YELLOWFIN',
          text: '(Thunnus albacares)',
          img: 'https://www.img.in.th/images/1290da0c16122517a4490995c8219f85.png',
        },
      ],
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
.slide{
  margin-left: 50px;
}

.pic{
  margin: 0px 60px 20px;
}

.media{
  width: 290px;
  height: 87px;
  font-family: Roboto;
  font-size: 60px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.5;
  letter-spacing: 6px;
  text-align: center;
  color: #ffffff;
  margin-top: 50px;
}
.size{
  width: 290px;
  height: 87px;
  font-family: Roboto;
  font-size: 60px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.5;
  letter-spacing: 6px;
  text-align: center;
  color: #ddc7a9;
  margin-top: 50px;
}
.text{
  width: 217px;
  height: 26px;
  text-align: left;
  color: #939393;
  margin-left: 39px;
}
.meatfont{
  width: 217px;
  height: 26px;
  color: #939393;
  text-align: center;
}

.font{
  color: #f9891b;
  text-align: center;
}
.fishpic{
  width: 353px;
  height: 113px;
  margin: 100px 0px 0px;
}
.title{
  font-family: Roboto;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.3;
  letter-spacing: 2px;
  text-align: left;
  margin-left: 30px;
  padding-top: 30px;
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

.SIZE {
  font-family: Roboto;
  font-size: 60px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.5;
  letter-spacing: 6px;
  text-align: center;
  color:#ddc7a9;
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
