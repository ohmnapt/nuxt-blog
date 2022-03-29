<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/admin/AdminPostForm.vue'
export default {
  layout: 'admin',
  components: {
    AdminPostForm,
  },
  data() {
    return {
      loadedPost: {
        author: 'Ohmnapt',
        title: 'My awesome',
        content: 'Super amazing my effort',
        thumbnailLink:
          'https://siambc.com/wp-content/uploads/2021/07/defi-scaled.jpg',
      },
    }
  },
}
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
