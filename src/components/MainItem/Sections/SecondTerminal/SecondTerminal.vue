<script setup lang="ts">
import { ref, onMounted } from "vue"

const now = new Date()
const options = <Record<string, string | boolean>>{
  year: "numeric",
  month: "2-digit",
  day: "2-digit",
  hour: "2-digit",
  minute: "2-digit",
  second: "2-digit",
  hour12: false,
}

const date = now.toLocaleString("en-GB", options)
</script>

<template>
  <section class="terminal">
    <div class="header">
      <div class="header--point point_red"></div>
      <div class="header--point point_yellow"></div>
      <div class="header--point point_green"></div>
    </div>
    <ul class="terminal--list">
      <li class="terminal--item">
        <p class="terminal--text">
          Last login: {{ date }} on ttys001 <br />
          Welcome to my portfolio terminal. <br />Type 'help' for a list of
          available commands.
        </p>
      </li>

      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ help</h4>
        <p class="terminal--text">
          Available commands: <br />
          about - Отобразить информацию о соискателе<br />
          skills - Список технических навыков<br />
          education - Отобразить профильное образования<br />
          <!-- experience - List work experience<br /> -->
          resume - Отобразить резюме<br />
          contact - Отобразить контактную информацию<br />
          <!-- clear - Clear the terminal screen<br /> -->
          exit - Выйти из терминала
        </p>
      </li>

      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ about</h4>
        <p class="terminal--text">
          Name: Симанков Роман<br />
          Age: 21<br />
          Location: Россия, Краснодар<br />
          Occupation: Фронтенд-разработчик<br />
        </p>
      </li>

      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ skills</h4>
        <p class="terminal--text">
          - HTML/CSS<br />
          - JavaScript<br />
          - TypeScript<br />
          - Vue.js<br />
          - React.js<br />
          - SCSS<br />
          - Git<br />
          - Адаптивная вёрстка
        </p>
      </li>

      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ education</h4>
        <p class="terminal--text">
          Education: <br />
          profession - Мастер по обработке цифровой информации 09.01.03.<br />
          educational institution - Новороссийский профессиональный техникум
        </p>
      </li>

      <!-- <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ experience</h4>
        <p class="terminal--text">
          Work Experience: <br />
          ---
        </p>
      </li> -->

      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ contact</h4>
        <p class="terminal--text">
          - Email:
          <a href="mailto:simanckovroman@gmail.com" class="terminal--link"
            >simanckovroman@gmail.com</a
          >
          <br />
          - Telegram:
          <a href="https://t.me/Cr0coDilda" class="terminal--link"
            >https://t.me/Cr0coDilda</a
          >
          <br />
          - GitHub:
          <a href="https://github.com/CrocoDilda" class="terminal--link"
            >https://github.com/CrocoDilda</a
          ><br />
          - hh.ru:
          <a
            href="https://hh.ru/resume/8a06b15eff0b75794d0039ed1f494d4c4b3977"
            class="terminal--link"
            >https://hh.ru/resume</a
          ><br />
        </p>
      </li>

      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ resume</h4>
        <p class="terminal--text">
          <a
            href="../../../../assets/Резюме_Frontend_разработчик_Роман_Симанков_от_04_10_2024_12_11.pdf"
            class="terminal--link"
            download
            >RomanSimanckov.pdf</a
          >
        </p>
      </li>
    </ul>
  </section>
</template>

<style scoped>
@import "./second-terminal.css";
</style>
