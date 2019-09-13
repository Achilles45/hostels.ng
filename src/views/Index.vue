<template>
  <div class="home">
    <Banner />
    <HomeHostels />
    <Process />
    <Ambassador />
    <ListHostel />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src

import Banner from '@/components/Banner.vue';
import HomeHostels from '@/components/HomeHostels.vue';
import Process from '@/components/Process.vue';
import Ambassador from '@/components/Ambassador.vue';
import ListHostel from '@/components/ListHostel.vue';
import Footer from '@/components/Footer.vue';
export default {
  name: 'index',
  components:{
    Banner,
    HomeHostels,
    Process,
    Ambassador,
    ListHostel,
    Footer
  }
}
</script>
