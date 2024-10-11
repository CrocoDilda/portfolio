<script setup lang="ts">
import ProjectsItem from "./ProjectsItem/ProjectsItem.vue"
import { projects } from "@/assets/projects-section"
</script>

<template>
  <section id="projects" class="projects">
    <h2 class="projects--title">Мои проекты</h2>

    <ul class="projects--list">
      <ProjectsItem
        v-for="project in projects"
        :key="project.id"
        :project="project"
      />
    </ul>
  </section>
</template>

<style scoped>
.projects {
  display: grid;
  justify-items: center;
  gap: 80px;
  margin-top: 50px;
  &:target {
    padding-top: 50px; /* Замените на нужный вам отступ */
  }
}

.projects--list {
  display: grid;
  gap: 80px;
}
</style>
