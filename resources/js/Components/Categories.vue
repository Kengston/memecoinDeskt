<template>
    <div class="p-5 bg-cream-medium rounded-lg shadow-sm">
        <h3 class="text-2xl font-semibold mb-4 text-cream-dark">Categories</h3>
        <ul class="space-y-2">
            <li v-for="(category, index) in categories" :key="index" class="flex items-center space-x-2 transition-colors duration-200 hover:text-cream-light cursor-pointer">
                <font-awesome-icon :icon="category.icon" class="fa-lg"/>
                <p class="text-cream-medium text-lg">{{ category.name }}</p>
            </li>
        </ul>
    </div>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faDog, faCat, faLandmark } from '@fortawesome/free-solid-svg-icons';

export default {
    data() {
        return {
            categories: [
                {name: 'Dogs', icon: faDog},
                {name: 'Cats', icon: faCat},
                {name: 'Politics', icon: faLandmark},
            ]
        }
    },
    components: {
        FontAwesomeIcon
    },
}
</script>

<style scoped>
.bg-cream-medium {
    background-color: #D7C4BB; /* Equivalent to Bone */
}

.text-cream-dark {
    color: #D7C4BB; /* Equivalent to Bone */
}

.text-cream-light {
    color: #F5F5DC; /* Equivalent to Ivory */
}

.hover\:text-cream-light:hover {
    color: #F5F5DC;
}
</style>
