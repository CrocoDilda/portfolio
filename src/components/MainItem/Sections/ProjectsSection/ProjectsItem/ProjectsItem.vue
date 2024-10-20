<script setup lang="ts">
import ArrovIcon from "@/components/icons/ArrovIcon.vue"
import GithubIcon from "@/components/icons/GithubIcon.vue"

type Obj = {
  title: string
  description: string
  image: string
  imageMobile: string
  liveDemoLink: string
  githubLink: string
  technologiesUsed: string[]
  id: number
}
const props = defineProps<{
  project: Obj
}>()

const imagePath = new URL(
  `../../../../../assets/images/${props.project.image}`,
  import.meta.url
).href

const imagePathMobile = new URL(
  `../../../../../assets/images/${props.project.imageMobile}`,
  import.meta.url
).href
</script>

<template>
  <li class="project">
    <picture>
      <source :srcset="`${imagePathMobile}`" media="(max-width: 1000px)" />
      <img class="project--image" :src="`${imagePath}`" alt="" />
    </picture>

    <div class="project--wrapper">
      <div class="project--triangles-wrapper">
        <div class="project--triangle triangle_1"></div>
        <div class="project--triangle triangle_2"></div>
        <div class="project--triangle triangle_3"></div>
      </div>
      <h3 class="project--title">{{ project.title }}</h3>
      <p v-html="project.description" class="project--description"></p>
      <ul class="project--list">
        <li
          v-for="tech in project.technologiesUsed"
          :key="tech"
          class="project--item"
        >
          {{ tech }}
        </li>
      </ul>
      <div class="project--links-wrapper">
        <a :href="project.liveDemoLink" target="_blank" class="project--link"
          >Live Demo <ArrovIcon class="project--link--icon" />
        </a>
        <a :href="project.githubLink" target="_blank" class="project--link">
          <GithubIcon class="project--link--icon" /> GitHub
        </a>
      </div>
    </div>
  </li>
</template>

<style scoped>
@import url(./projects-item.css);
</style>
