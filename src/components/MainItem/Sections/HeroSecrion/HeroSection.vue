<script setup lang="ts">
import { ref, onMounted } from "vue"

const titleSteps = ref(15)

onMounted(() => {
  const title = document.querySelector("[data-title]") as HTMLElement
  titleSteps.value = title.innerText.length
})
</script>

<template>
  <section class="hero">
    <div class="hero--inner">
      <p class="hero--title">></p>
      <h1
        :style="`animation: title 8s linear infinite; animation-timing-function: steps(${titleSteps});`"
        data-title="Roman Simanckov"
        class="hero--title title"
      >
        Roman Simanckov
      </h1>
      <div class="cursor"></div>
    </div>
    <p class="big-text">
      Я фронтенд-разработчик, работаю с фреймворками Vue и React. Создаю
      производительные, адаптивные и масштабируемые веб-приложения,
      ориентированные на решение конкретных задач. Ознакомьтесь с моими
      <a href="#projects" class="hero--link">проектами</a> ниже.
    </p>
  </section>
</template>

<style scoped>
@import url(./hero-section.css);
</style>
