<template>
  <section class="posts-list">
    <PostPreview
      id="1"
      thumbnail="https://media.mehrnews.com/d/2018/10/28/4/2940617.jpg"
      title="Hello there!"
      previewText="This is my first post!"
    />
    <PostPreview
      id="2"
      thumbnail="https://media.mehrnews.com/d/2018/10/28/4/2940617.jpg"
      title="Hello there! 2nd"
      previewText="This is my 2nd post!"
    />
    <PostPreview
      id="3"
      thumbnail="https://media.mehrnews.com/d/2018/10/28/4/2940617.jpg"
      title="Hello there! 3rd"
      previewText="This is my 3rd post!"
    />
  </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview';
export default {
  components: {
    PostPreview,
  },
};
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
