<template>
  <div class="body">
    
    <div class="bg">
      <Header></Header>
      <!-- <v-img class="marginImg" max-height="1161px" max-width="1490px" src="../assets/designer_1.png"></v-img> -->
      <v-card flat solo class="bgTrans margin2">
        <p class="fontContent-a">Introduce Your Product Quickly & Effectively</p>
        <p class="fontContent-a2">Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
        Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes,
        nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat
        massa quis enim.</p>
        <v-row class="margin1">
          <v-btn class="me-8 fontContent-a3" color="#111B47">Purchase UI Kit</v-btn>
          <v-btn class="fontContent-a3" color="black" outlined>Learn More</v-btn>
        </v-row>
      </v-card>
    </div>

    <div class="">
      <v-row>
        <v-col class="margin3" cols="12" sm="12" md="12" lg="6" xl="6">
          <v-card flat solo class="margin2">
            <p class="fontContent-b1 ">Light, Fast & Powerful</p>
            <p class="fontContent-b2 ">Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.
            Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus 
            mus.<br>
            Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa 
            quis enim.</p>

            <v-row>
              <v-col cols="6">
                <v-img width="255px" height="36px" src="../assets/Left.png"></v-img>
                <p class="fontContent-b3 mt-3" style="max-width: 255px; ">Title Goes Here</p>
                <p class="fontContent-b4 mt-1" style="max-width: 255px; ">Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. </p>
              </v-col>

              <v-col cols="6">
                <v-img width="255px" height="36px" src="../assets/Left.png"></v-img>
                <p class="fontContent-b3 mt-3" style="max-width: 255px; ">Title Goes Here</p>
                <p class="fontContent-b4 mt-1" style="max-width: 255px; ">Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
                Aenean commodo ligula eget dolor. </p>
              </v-col>
            </v-row>
          </v-card>
        </v-col>

        <v-col class="margin4" cols="12" sm="12" md="12" lg="6" xl="6">
          <v-img max-width="540px" src="../assets/mobile.png"></v-img>
        </v-col>
      </v-row>
    </div>

    <div>
      <Element mw="480" :url="pUrl1" :prop-text1="text1" :prop-text2="text1a" :show-prop="false"></Element>
      <Element mw="540" :url="pUrl2" :prop-text1="text2" :prop-text2="text2a" :show-prop="false"></Element>
      <Element mw="445" :url="pUrl3" :prop-text1="text3" :prop-text2="text3a" :show-prop="true"></Element>
    </div>

    <div class="bg2">
      <v-card flat style="height: 100%; background: transparent;" class="d-flex justify-center align-center flex-column">
        <p class="fontContent-b1">A Price To Suit Everyone</p>
        <p class="text-center fontContent-b2 mt-4">Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
        Aenean commodo ligula eget dolor. Aenean massa. 
        Cum sociis natoque penatibus et magnis dis parturient montes,
        nascetur ridiculus </p>
        <p class="mt-9 fontContent-d1">40$</p>
        <p class="fontContent-b2">UI Design Kit</p>
        <p class="mt-15 fontContent-d2">See, One price. Simple.</p>
        <v-btn width="189" color="#111B47" class="fontContent-d2" style="color: white !important; text-transform: capitalize;">Purchase Now</v-btn>
      </v-card>
    </div>

    <div>
      <Footer></Footer>
    </div>
  </div>
</template>

<script>
import header from '../components/Header.vue';
import footer from '../components/Footer.vue';
import element from '../components/Element.vue';

export default {

  name: 'home-page',
  components: {
    'Header' : header,
    'Footer' : footer, 
    'Element' : element,
  },

  data (){
    return{
      pUrl1 : require ('../assets/pic1.png'),
      pUrl2 : require ('../assets/pic2.png'),
      pUrl3 : require ('../assets/pic3.png'),
      text1 : "Light, Fast & Powerful",
      text2 : "Light, Fast & Powerful",
      text3 : "Light, Fast & Powerful",
      text1a : "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim.",
      text2a : "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim.",
      text3a : "Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim.",

    }
  },

  methods : {

  },

  created(){

  },
}

</script>

<style>
.body{
  width:100%;
}

.bg{
  background-image: url(../assets/designer_1.png);
  background-size: 60% 120%;
  background-position: right;
  height:auto;
  padding-bottom: 400px;
}

.bg2{
  background-image: url(../assets/Rectangle.png);
  background-position: center;
  background-size: 100% 100%;
  height:1000px;
}

.bgTrans{
  background: transparent !important;
}

.margin1{
  margin-top: 74px !important;
}

.margin2{
  margin-left: 165px;
}

.margin3{
  margin-top: 160px;
}

.margin4{
  display:flex;
  margin-top: 110px;
  justify-content: center;
}

.fontContent-a{
  font-family: Roboto;
  font-size: 50px;
  font-style: normal;
  font-weight: 500;
  line-height: 66px; /* 132% */
  letter-spacing: 1px;
  max-width: 539px;
  margin-top: 303px;
}

.fontContent-a2{
  font-family: Roboto;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 30px; /* 166.667% */
  max-width: 539px;
  margin-top: 20px;
  color:#505F98;
}

.fontContent-a3{
  font-family: Roboto;
  font-size: 16px !important;
  font-style: normal;
  font-weight: 500;
  line-height: 26px; /* 162.5% */
  color: white !important;
  text-transform: capitalize;
  width: 189px;
}

.fontContent-b1{
  font-family: Roboto;
  font-size: 36px;
  font-style: normal;
  font-weight: 500;
  line-height: 48px; /* 133.333% */
  max-width: 589px;
}

.fontContent-b2{
  font-family: Roboto;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 26px; /* 162.5% */
  max-width: 540px;
  color:#505F98;
}

.fontContent-b3{
  font-family: Roboto;
  font-size: 16px;
  font-style: normal;
  font-weight: bold;
  line-height: 26px; /* 162.5% */
}

.fontContent-b4{
  font-family: Roboto;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: 18px; /* 150% */
}

.fontContent-d1{
  font-family: Roboto;
  font-size: 50px;
  font-style: normal;
  font-weight: 500;
  line-height: 66px; /* 132% */
  letter-spacing: 1px;
}

.fontContent-d2{
  font-family: Roboto;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px; /* 171.429% */
  color:#505F98;
}

</style>