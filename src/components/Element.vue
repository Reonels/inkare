<template>
  <div class="marginElement">
    <v-row class="marginRow">
      <v-col class="marginCol">
        <v-img class="" :max-width="mw" :max-height="mh" :src="url"></v-img>
      </v-col>

      <v-col class="marginCol2">
        <div>
        <p class="fontContent-c1">{{ propText1 }}</p>
        <p style="color:#505F98;" class="fontContent-c2 mt-4">{{ propText2 }}</p>
        <v-btn class="fontContent-c3 mt-11" v-if="showProp" color="#111B47">purchase now</v-btn>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>

export default {
  props : ['mw','url','propText1','propText2' ,'showProp'],

  name: 'element-page',

  data (){
    return{

    }
  },

  methods : {

  },

  created(){

  },
}

</script>

<style>
.marginElement{
  margin : 0px 165px;
}

.marginRow{
  margin : 172px 0px;
}

.marginCol{
  display: flex;
  justify-content: center;
  align-items: center;
}

.marginCol2{
  display: flex;
  justify-content: center;
  align-items: center;
}

.fontContent-c1{
  font-family: Roboto;
  font-size: 36px;
  font-style: normal;
  font-weight: 500;
  line-height: 48px; /* 133.333% */
  max-width: 445px;
}

.fontContent-c2{
  font-family: Roboto;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 26px; /* 162.5% */
  max-width: 445px;
}

.fontContent-c3{
  font-family: Roboto;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px; /* 171.429% */
  text-transform: capitalize;
  color: white !important;
}

</style>