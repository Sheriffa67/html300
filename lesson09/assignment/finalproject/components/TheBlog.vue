<template>
  <div class="add-blog">
    <h2>Add a new Blog Post</h2>
    <form>
      <label>Blog Title</label>
      <input type="text" v-model.lazy="blog.title" required />
      <label>Blog Content:</label>
      <textarea v-model.lazy="blog.content"></textarea>
    </form>
    <div id="preview">
        <h3>Preview Blog</h3>
        <p>Blog title:{{blog.title}}</p>
        <p>Blog content:</p>
        <p>{{blog.content}}</p>
    </div>
  </div>

</template>

<script>
export default {
  data() {
    return {
      blog: {
        title: "",
        content: "",
      }
    }
  },
  methods:{

  }
}
</script>

<style lang="css" scoped>
</style>
