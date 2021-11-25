<template>
<div class="main">
  <div class="logo">
    <h1 class="title">ANIMES DS</h1>
  </div>

  <div class="header"></div>

  <Header />
  <Body />
  <Footer />

  <div class="body"></div>
  <div class="footer"></div>
  </div>
</template>

<script>

// eslint-disable-next-line import/no-unresolved
import Header from '@/components/Header.vue';
import Body from '@/components/Body.vue';
import Footer from '@/components/Footer.vue';

export default {
  components: {
    Header, Body, Footer,
  },
};
</script>

<style lang ="scss">
.main{
  height: 100vh;
  display: flex;
  flex-direction: column;
  font-family: sans-serif;
  background-color: black;
}
.title{font-size: 50px;}
.header{
  display: flex;
  justify-content: space-between;
  padding: 20px;
  background-color: black;
}
a{
  text-decoration: none;
  font-weight: bold;
  color: gray;
}
.logo{align-self: center; color: rgb(199, 3, 3); text-shadow: 1px 5px 10px rgb(66, 66, 66);}
.xp{padding: 10px; background-color: black;}
.body{flex-grow: 1; background-color: rgb(0, 0, 0);
display: flex; flex-wrap: wrap; justify-content: space-around; padding-top: 50px;
}
.searchbox{ display: flex; align-self: center;
padding-bottom: 10px; width: 230px; border: 1px solid rgb(0, 0, 0);
border-radius: 20px; height: 30px;align-items: center;
justify-items: center ; background-color: black; padding-left: 30px;
border: 1px solid gray;

}
.animebox{ height: 200px; width: 300px; margin-top: 25px; margin-bottom: 25px;
box-shadow: 1px 1px 10px 5px rgba(61, 61, 61, 0.692);
}
.lupa{
margin-top: 10px;

}
.textbox{
background-color: black;
padding-left: 20px;
padding-right: 15px;
margin-top: 10px;
outline: none;
border: none;
width: 150px;
height: 15px;
}
.img{ height: 200px; width: 300px;}
.footer{display: flex; justify-content: center; background-color: black; color: white;}
</style>
