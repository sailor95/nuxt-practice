<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm';

export default {
  name: 'AdminPostId',
  layout: 'admin',
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        author: 'Dave',
        title: 'Good Book',
        content: 'Super amazing book!',
        thumbnailLink: 'https://media.mehrnews.com/d/2018/10/28/4/2940617.jpg',
      },
    };
  },
};
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}
@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
