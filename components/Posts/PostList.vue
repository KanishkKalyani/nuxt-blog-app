<template>
  <section class="post-list">
    <PostPreview
      :id="'1'"
      :is-admin="isAdmin"
      :thumbnail="'https://www.hydrocarbons-technology.com/wp-content/uploads/sites/9/2020/09/shutterstock_1152185600-1440x1008-1-857x600.jpg'"
      :title="'Post 1'"
      :previewText="'Post 1 Preview'"
    ></PostPreview>
    <PostPreview
      :id="'2'"
      :is-admin="isAdmin"
      :thumbnail="'https://www.hydrocarbons-technology.com/wp-content/uploads/sites/9/2020/09/shutterstock_1152185600-1440x1008-1-857x600.jpg'"
      :title="'Post 2'"
      :previewText="'Post 2 Preview'"
    ></PostPreview>
    <PostPreview
      :id="'3'"
      :is-admin="isAdmin"
      :thumbnail="'https://www.hydrocarbons-technology.com/wp-content/uploads/sites/9/2020/09/shutterstock_1152185600-1440x1008-1-857x600.jpg'"
      :title="'Post 3'"
      :previewText="'Post 3 Preview'"
    ></PostPreview>
  </section>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview";

export default {
  components: {
    PostPreview,
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
