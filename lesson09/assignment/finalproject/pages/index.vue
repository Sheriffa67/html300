<template>
  <div class="container">
    <div class="navbar">
        <TheNavigation />
    </div>
    <h1>The one place for all your traveling need</h1>
    <p>From Brazil to africa, you can find information on how to travel</p>

    <footer>
      <TheNavigation />
    </footer>
  </div>

</template>

<script>

import TheNavigation from "@/components/TheNavigation";
import TheBlog from "@/components/TheBlog";


export default {
  components: {
    TheNavigation
  },
  // components: {
  //   TheBlog
  // }

//  data: function () {
//    return {
//      pics: [
//        {url: require('assets/brazil.jpg'), alt: 'Picture of Brazil'},
//        {url: require('assets/hawaii.jpg'), alt: 'picture of hawaii'},
//        {url: require('assets/jamaica.jpg'), alt: 'picture of jamaica'},
//        {url: require('assets/panama.jpg'), alt: 'picture of panama'},
//      ]
//    }
//  }
};

</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
}
</style>
