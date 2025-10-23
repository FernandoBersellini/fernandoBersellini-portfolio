<script setup>
    const props = defineProps({
        projectName: String,
        projectDescription: String,
        technologies: Array,
        repoLink: String
    });

</script>

<template>
    <div class="radius shadow-lg p-4 m-2 flex flex-col gap-2">
        <h1 class="text-center">{{props.projectName}}</h1>
        <p>{{ props.projectDescription }}</p>
        <ul>
            <li v-for="tech in props.technologies" :key="tech">{{ tech }}</li>
        </ul>
        <a :href="props.repoLink">Link do repositorio</a>
    </div>
</template>