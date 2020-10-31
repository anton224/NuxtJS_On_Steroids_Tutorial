<template>
    <section class="post-list">      
        <PostPreview 
        id="1"
        :is-admin="isAdmin"
        thumbnail="https://www.tech-il.co.il/wp-content/uploads/2020/10/computing-tech-main.jpg"
        title="Hello there!"
        previewText="This is my 1 post!"
        />
        <PostPreview 
        id="2"
        :is-admin="isAdmin"
        thumbnail="https://www.tech-il.co.il/wp-content/uploads/2020/10/computing-tech-main.jpg"
        title="Hello there! 2"
        previewText="This is my 2 post!"
        />
        <PostPreview 
        id="3"
        :is-admin="isAdmin"
        thumbnail="https://www.tech-il.co.il/wp-content/uploads/2020/10/computing-tech-main.jpg"
        title="Hello there! 3"
        previewText="This is my 3 post!"
        />
        </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
    components:{
        PostPreview
    },
    props: {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
}
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