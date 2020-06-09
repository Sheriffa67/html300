<template>
  <nav id="nav">
    <h1>{{title}}</h1>
    <ul>
      <li><nuxt-link to="/">Home</nuxt-link></li>
      <li><nuxt-link to="/brazil">Brazil</nuxt-link></li>
      <li><nuxt-link to="/hawaii">Hawaii</nuxt-link></li>
      <li><nuxt-link to="/jamaica">Jamaica</nuxt-link></li>
      <li><nuxt-link to="/panama">Panama</nuxt-link></li>
    </ul>
  </nav>

</template>

<script>
  export default {
    data () {
      return {
        title: 'Lets Travel!'
      }
    },
    head () {
    return {
      title: this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: 'My custom description' }
      ]
    }
  }
}
</script>

<style scoped>
 #nav {
   display: flex;
   flex-direction: row;
   padding: 30px;
 }

 #nav a {
   font-weight: bold;
   color: #2c3e50;
   padding: 0 10px;
 }

 #nav a.vue-school-active-class {
   color: #ab26ab;
 }
 li {
   list-style: none;
   display: inline;
   padding: 0;
   overflow: hidden;
   background-color: white;
}

li {
  float: left;
}

li {
  display: block;
  color: white;
  text-align: center;
  padding: 10px;
  text-decoration: none;
}

li:hover {
  background-color: aqua;
}
 </style>
