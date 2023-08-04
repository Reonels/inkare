<template>
  <div class="bg3">
    <v-row style="height: 140px;" class="marginElement d-flex justify-space-between align-center">
      <p class="fontContent-e1"> <span>&copy;</span> 2023 Yourcompany</p>
      <li class="headCenter"><a>Landing</a></li>
      <v-hover v-slot="{hover}">
        <v-btn class="fontBtn" :style="{'background-color':hover ? '#FFB84C' : '#111B47'}" width="109">Purchase now</v-btn>
      </v-hover>
    </v-row>

    <hr class="marginElement">

    <v-row class="marginElement">
      <v-col class="px-0">
        <v-toolbar-items class="headLeft">
          <li class="ps-0"><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </v-toolbar-items>

      </v-col>

      <v-col>
        <v-row class="justify-end my-auto">
          <div class="mx-4">
            <v-img width="16" height="16" src="../assets/fb.png"></v-img>
          </div>

          <div class="mx-4">
            <v-img width="16" height="16" src="../assets/link.png"></v-img>
          </div> 

          <div class="mx-4">
            <v-img width="16" height="16" src="../assets/tw.png"></v-img>
          </div>

          <div class="mx-4">
            <v-img width="16" height="16" src="../assets/yt.png"></v-img>
          </div> 

          <div class="ms-4 me-0">
            <v-img width="16" height="16" src="../assets/ig.png"></v-img>
          </div>
        </v-row>
      </v-col>
    </v-row>
  </div>
</template>

<script>

export default {

  name: 'footer-page',

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
.bg3{
  background-color: #E7ECFF;
  height: 220px;
}

.fontContent-e1{
  font-family: Roboto;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px; /* 171.429% */
  color:#939EA4;
}

</style>