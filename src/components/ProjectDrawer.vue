<template lang="">
    <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
        <div class="offcanvas-header">
            <h5 class="offcanvas-title" id="offcanvasExampleLabel"></h5>
            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
            <div>
                <h3>{{ item.title }}</h3>
                <a :href="item.link" target="_blank"><img :src="getImageSrc(item.image)" :alt="item.title"></a>
                <p>👉 <a :href="item.link" target="_blank">{{ item.link }}</a></p>
                <p>{{ item.description }}</p>
                <p>Features:</p>
                <ul v-for="feature in item.features">
                    <li>{{ feature }}</li>
                </ul>
                <p>🔥 Made with: <span v-for="(tech, index) in item.technologies" :key="index">{{ tech }}{{ index !== item.technologies.length - 1 ? ', ' : '' }}</span></p>
            </div>
        </div>
    </div>
</template>

<script setup>
    import { defineProps } from 'vue';

    const props = defineProps({
        item: {
            type: Object,
            required: true,
        }
    });

    const getImageSrc = (imageName) => {
        return new URL(`../assets/img/projects/${imageName}`, import.meta.url).href;
    };
</script>

<style lang="">
    
</style>