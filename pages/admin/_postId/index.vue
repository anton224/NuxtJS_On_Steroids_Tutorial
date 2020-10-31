<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost" />
        </section>
    </div>
</template>

<script>
import AdminPostForm from '@/components/admin/AdminPostForm'

export default {
    components: {
        AdminPostForm
    },
    data() {
        return {
            loadedPost: {
                author: 'Mike',
                title: 'My Post',
                content: 'Fun Post',
                thumbnail: 'https://www.tech-il.co.il/wp-content/uploads/2020/10/computing-tech-main.jpg'
            }
        }
    },
    layout: 'admin'
}
</script>
<style scoped>
.update-form{
    width: 90%;
    margin: 20px auto;
}
@media (min-width: 768px) {
    .update-form{
        width: 500px;
    }
}
</style>