<template>
  <section id="posts">
    <PostPreview
      v-for="post in posts"
      :key="post.id"
      :title="post.title"
      :excerpt="post.previewText"
      :thumbnailImage="post.thumbUrl"
      :id="post.id"
    />
  </section>
</template>

<script>
import PostPreview from '@/components/Blog/PostPreview'
export default {
  components: {
    PostPreview
  },
  data() {
    return {
      posts: [
        {
          title: 'Пост про лисички',
          previewText: 'Это текст для превьюхи c лисичками',
          thumbUrl: 'https://i.pinimg.com/originals/0f/fd/dd/0ffddd32f693c21bebdacda949d231be.jpg',
          id: 'a-foxy-post'
        },
        {
          title: 'Пост про диоды',
          previewText: 'Это текст для превьюхи c лисичками',
          thumbUrl: 'https://i.pinimg.com/originals/0f/fd/dd/0ffddd32f693c21bebdacda949d231be.jpg',
          id: 'a-diod-post'
        },
        {
          title: 'Пост про диоды',
          previewText: 'Это текст для превьюхи c лисичками',
          thumbUrl: 'https://i.pinimg.com/originals/0f/fd/dd/0ffddd32f693c21bebdacda949d231be.jpg',
          id: 'a-diod-post'
        }
      ]
    }
  }
}
</script>

<style scoped>
#posts {
  padding-top: 2rem;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-direction: column;
}
@media (min-width: 35rem) {
  #posts {
    flex-direction: row;
  }
}
</style>
