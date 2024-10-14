<template>
  <section class="terminal">
    <div class="header">
      <div class="header--point point_red"></div>
      <div class="header--point point_yellow"></div>
      <div class="header--point point_green"></div>
    </div>
    <ul class="terminal--list">
      <li class="terminal--item">
        <h4 class="terminal--tile">roman@portfolio:~$ show characteristics</h4>
        <p class="terminal--text"></p>
      </li>
      <li class="terminal--item">
        <h4 class="terminal--tile">Roman.currentLocation</h4>
        <p class="terminal--text">"Россия, Краснодар"</p>
      </li>
      <li class="terminal--item">
        <h4 class="terminal--tile">Roman.contactInfo</h4>
        <p class="terminal--text">
          ["<a
            target="_blank"
            href="mailto:simanckovroman@gmail.com"
            class="terminal--link"
            >simanckovroman@gmail.com</a
          >", "<a
            target="_blank"
            href="https://t.me/Cr0coDilda"
            class="terminal--link"
            >Telegram</a
          >", "
          <a
            target="_blank"
            href="https://github.com/CrocoDilda"
            class="terminal--link"
            >GitHub</a
          >", "<a
            target="_blank"
            href="https://hh.ru/resume/8a06b15eff0b75794d0039ed1f494d4c4b3977"
            class="terminal--link"
            >hh.ru</a
          >"]
        </p>
      </li>
      <li class="terminal--item">
        <h4 class="terminal--tile">Roman.resume</h4>
        <p class="terminal--text">
          "<a
            target="_blank"
            href="../../../../../public/Резюме_Frontend_разработчик_Роман_Симанков_от_04_10_2024_12_11.pdf"
            class="terminal--link"
            download
            >RomanSimanckov.pdf</a
          >"
        </p>
      </li>
      <li class="terminal--item">
        <h4 class="terminal--tile">Roman.education</h4>
        <p class="terminal--text">
          Мастер по обработке цифровой информации 09.01.03. Новороссийский
          профессиональный техникум
        </p>
      </li>
      <li class="terminal--item">
        <h4 class="terminal--tile">Roman.skills</h4>
        <p class="terminal--text">
          ["HTML", "CSS", "JavaScript", "Vue", "React", "TypeScript", "SCSS",
          "Git", "Адаптивная вёрстка"]
        </p>
      </li>
      <li class="terminal--item">
        <h4 class="terminal--tile"><div class="terminal--cursor"></div></h4>
      </li>
    </ul>
  </section>
</template>

<style scoped>
@import "./terminal-section.css";
</style>
