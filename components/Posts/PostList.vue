<template>
     <section class="featured-posts">
     <PostPreview
     id="1"
     :is-admin="isAdmin"
     thumbnail="https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
     title="hello there"
     previewText="this is my first post"/>
      
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
    components: {
        PostPreview
    },
    props : {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style scoped>

.post-lists {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>