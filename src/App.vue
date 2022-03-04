<template>
<div class="wrapper">
  <div id="nav">
  <Header />
  </div>
  <router-view />
</div>
<Footer />
</template>
<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
export default {
  components : {
    Header,
    Footer,
  }
}
</script>
<style>

@font-face {
  font-family: "DINPro-Bold";
  src: 
    url("assets/fonts/DINPro-Bold.woff") format("woff"),
    url("assets/fonts/DINPro-Bold.ttf") format("truetype");
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}
@font-face {
  font-family: "DINPro-Medium";
  src: 
    url("assets/fonts/DINPro-Medium.woff") format("woff"),
    url("assets/fonts/DINPro-Medium.ttf") format("truetype");
  font-weight: 100;
  font-style: normal;
  font-display: swap;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 1024px;
  margin: 0px auto;
  position: relative;
  border: 1px solid #97979791;
  border-top:0px;
  border-bottom: 0px;
}
.wrapper{
  padding: 0 30px;
}
#nav {
  padding:30px 0;
  
}
div#collapseExample{
  z-index: 5555;
}
#nav a {
 /* font-weight: bold;*/
 font-family: "DINPro-Medium";
  color: #222222;
  text-align: left;
  font-size: 57px;
/*  width: 100%;*/
  text-decoration: none;
  border-bottom: 1px solid #c0c0c054;
  letter-spacing: 0.02em;
}

#nav a:hover{
  text-decoration: underline;
}
.card.card-body {
    border: 0;
    box-shadow: 0px 3px 0px 0px #6e676761;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
div#collapseExample {
    position: absolute;
    width: 100%;
    left: 0;
     top: 0%;
}


@media (max-width: 768px) {
  .row{
      display: grid;
      grid-template-columns: 61% 45%;
  }
  .logo {
      margin-top: 8px;
  }
  #nav {
    padding: 10px;
  }
  #app{
    margin: 0px;
    width: 100%;
    padding: 0 10px;
  }
  .artists_box:last-child{
    display: none;
  }
  .wrapper{
    padding: 0 0px;
  }
  div#collapseExample{
    top: 0%;
  }
  .searchs {
    position: absolute;
    left: 0;
  }
  .form-control{
    width: 91%;
  }
}

</style>
