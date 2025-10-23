<script setup>
    import ProjectCard from './ProjectCard.vue';
</script>

<template>
    <div class="mt-50">
        <h1 class="text-center">Project section</h1>
        <div class="m-auto w-1/2 grid grid-cols-2 gap-5">
            <ProjectCard
                projectName="Project 1"
                projectDescription="Description for Project 1"
                :technologies="['Vue.js', 'Tailwind CSS', 'JavaScript']"
                repoLink="https://github.com/FernandoBersellini/DietInfo"
            />
            <ProjectCard />
            <ProjectCard />
        </div>
    </div>
</template>