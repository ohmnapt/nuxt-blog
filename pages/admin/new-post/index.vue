<template>
  <div class="admin0new-post-page">
    <section class="new-post-form">
      <AdminPostForm />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/admin/AdminPostForm.vue'

export default {
  components: {
    AdminPostForm,
  },
}
</script>
