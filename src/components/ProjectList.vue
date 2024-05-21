<template lang="">
    <div class="grid-container">
        <div @click="openDrawer(item)" v-for="item in items"
            data-bs-toggle="offcanvas" 
            data-bs-target="#offcanvasExample" 
            aria-controls="offcanvasExample"
            class="grid-item" 
            :style="{ background: `url(${getImageSrc(item.image)}) center/cover no-repeat`, filter: 'grayscale(1)' }"
        >
            <p>{{ item.title }}</p>
        </div>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';
import { defineEmits } from 'vue';

const props = defineProps({
    items: {
        type: Array,
        required: true,
    },
});

const emit = defineEmits(['projectSelected']);

const getImageSrc = (imageName) => {
    return new URL(`../assets/img/projects/${imageName}`, import.meta.url).href;
};

const openDrawer = (item) => {
    emit('projectSelected', item);
    console.log(item);
};

</script>

<style lang="">
    
</style>