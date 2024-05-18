<template lang="">
    <div class="grid-container">
        <div v-for="item in items" class="grid-item">
            <img :src="getImageSrc(item.image)" :alt="item.name">
            <p>{{item.name}}</p>
        </div>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    items: {
        type: Array,
        required: true,
    },
});

const getImageSrc = (imageName) => {
    return new URL(`../assets/img/tech/${imageName}`, import.meta.url).href;
};
</script>

<style lang="" scoped>
    
</style>