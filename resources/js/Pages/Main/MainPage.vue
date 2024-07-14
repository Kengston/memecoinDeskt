<template>
    <div class="main-page">
        <Header />
        <div class="main-content flex">
            <Categories class="w-1/4"/>
            <div class="w-3/4">
                <div v-for="(post, index) in posts" :key="index">
                    <h3>{{ post.title }}</h3>

                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Header from "@/Components/Header.vue";
import Categories from '@/Components/Categories.vue'
export default {
    components: {
        Header,
        Categories
    },

    props: {
        posts: Object,
    },
}
</script>
