<template>
  <div class="home">
    <Slider />
    <NewsEvents />
    <Channel />
    <Artists />
    <img alt="Vue logo" src="../assets/logo.png" />
    
  </div>
</template>

<script>
import Slider from "@/components/Slider.vue";
import NewsEvents from "@/components/NewsEvents.vue";
import Channel from "@/components/Channel.vue";
import Artists from "@/components/Artists.vue";


export default {
  name: "Home",
  components: {
 
    Slider,
    NewsEvents,
    Channel,
    Artists,

  },
};
</script>
