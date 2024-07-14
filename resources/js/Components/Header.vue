<template>
    <header class="bg-cream-light py-3 px-4">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="text-3xl font-semibold text-cream-dark">
                <a href="/">
                    Meme Desk
                </a>
            </h1>
            <nav>
                <ul class="flex items-center">
                    <li>
                        <button class="bg-cream-dark rounded-full p-2 mx-3 text-cream-light hover:bg-cream-medium transition-colors duration-300">
                            <font-awesome-icon icon="search"></font-awesome-icon>
                            Search
                        </button>
                    </li>
                    <li>
                        <button class="bg-cream-dark rounded-full p-2 mx-3 text-cream-light hover:bg-cream-medium transition-colors duration-300">
                            <font-awesome-icon icon="pencil"></font-awesome-icon>
                            Write
                        </button>
                    </li>
                    <li>
                        <button class="bg-cream-dark rounded-full p-2 mx-3 text-cream-light hover:bg-cream-medium transition-colors duration-300">
                            <font-awesome-icon icon="user"></font-awesome-icon>
                            Login
                        </button>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>

// Import the necessary libraries
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { library } from '@fortawesome/fontawesome-svg-core';
import { faSearch, faPencil, faUser } from '@fortawesome/free-solid-svg-icons';

library.add(faSearch, faPencil, faUser);
export default {
    name: 'Header',
    FontAwesomeIcon, // Declare FontAwesomeIcon component
}
</script>

<style scoped>
.bg-cream-light {
    background-color: #F5F5DC; /* Equivalent to Ivory */
}
.bg-cream-dark {
    background-color: #D7C4BB; /* Equivalent to Bone */
}
.bg-cream-medium {
    background-color: #EEE8AA; /* Equivalent to Pale Goldenrod for hover state */
}
.text-cream-dark {
    color: #D7C4BB; /* Equivalent to Bone */
}
.text-cream-light {
    color: #F5F5DC; /* Equivalent to Ivory */
}
</style>
