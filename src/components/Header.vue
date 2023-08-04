<template>
  <v-toolbar class="marginElement2" flat style="background: transparent;">
    <v-toolbar-items class="headLeft">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </v-toolbar-items>
    <v-spacer class=""></v-spacer>

    <v-toolbar-title class="headCenter">
      <li><a href="#">Landing</a></li>
    </v-toolbar-title>
    <v-spacer class="hidden-sm-and-down"></v-spacer>

    <v-toolbar-items class="headRight">
      <li class="">
        <v-hover v-slot="{hover}">
          <v-btn class="fontBtn" width="160px" :style="{'background-color':hover ? '#FFB84C' : '#111B47'}">Buy Now</v-btn>
        </v-hover>
      </li>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>

export default {

  name: 'header-page',

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
.marginElement2{
  margin : 0px 149px;
}

.headLeft{
  font-family: Roboto;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px; /* 171.429% */
  align-items: center;
}

.headCenter{
  font-family: Roboto;
  font-size: 26px;
  font-style: normal;
  font-weight: 900;
  line-height: 38px; /* 146.154% */
}

.headRight{
  align-items: center;
}

.fontBtn{
  color: white !important;
  font-size: 12px !important;
  text-transform: capitalize;
  font-family: Roboto;
  font-style: normal;
  font-weight: 500;
  line-height: 18px; /* 150% */
}

li{
  display: inline; 
  padding: 0px 20px;
}

a{
  color:#505F98 !important;
  text-decoration:none;
}

a:hover{
  color: #FFB84C!important;
}

</style>