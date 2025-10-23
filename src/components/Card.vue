<script setup>
    const props = defineProps({
        imageSrc: String,
        title: String
    });

    const imageUrl = props.imageSrc;
    const technolgyName = props.title;

</script>

<template>
    <div class="w-1/6 flex flex-nowrap justify-between radius shadow-lg p-4 m-2">
        <img class="size-20" :src="imageUrl" alt="">
          

        <h1 class="self-center">{{technolgyName}}</h1>
    </div>
</template>

<style scoped>
</style>