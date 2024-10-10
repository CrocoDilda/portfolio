<script setup lang="ts">
import ProjectsItem from "./ProjectsItem/ProjectsItem.vue"
import { projects } from "@/assets/projects-section"
</script>

<template>
  <div class="projects">
    <h2 class="projects--title">Мои проекты</h2>

    <ul class="projects--list">
      <ProjectsItem
        v-for="project in projects"
        :key="project.id"
        :project="project"
      />
    </ul>
  </div>
</template>

<style scoped>
.projects {
  display: grid;
  justify-items: center;
  gap: 80px;
  padding-bottom: 100px;
}

.projects--list {
  display: grid;
  gap: 80px;
}
</style>
