<!--In Vue.js, computed properties enable you to create a property that can be used to modify, manipulate, 
    and display data within your components in a readable and efficient manner.-->
<template>
        <p>Has Published Book:</p>
        <span>{{author.books.length > 0 ? 'Yes' : 'No'}}</span>
</template>

<script>
export default {
  data() {
    return {
      author: {
        name: 'John Doe',
        books: [
          'Vue 2 - Advanced Guide',
          'Vue 3 - Basic Guide',
          'Vue 4 - The Mystery'
        ]
      }
    }
  },
  computed: {
    publishedBooksMessage() {
      return this.author.books.length > 0 ? 'Yes' : 'No'
    }
  }
}

</script>

<style>

</style>