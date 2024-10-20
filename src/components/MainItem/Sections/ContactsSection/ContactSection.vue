<template>
  <section id="contacts" class="contacts">
    <h2 class="contacts--title">Мои контакты</h2>
    <ul class="contacts--list">
      <li class="contacts--item">
        <a
          target="_blank"
          href="mailto:simanckovroman@gmail.com"
          class="big-text big--link"
          >simanckovroman@gmail.com</a
        >
      </li>
      <li class="contacts--item lines">||</li>
      <li class="contacts--item">
        <a
          target="_blank"
          href="https://t.me/Cr0coDilda"
          class="big-text big--link"
          >Telegram</a
        >
      </li>
      <li class="contacts--item lines">||</li>
      <li class="contacts--item">
        <a
          target="_blank"
          href="https://github.com/CrocoDilda"
          class="big-text big--link"
          >GitHub</a
        >
      </li>
      <li class="contacts--item lines">||</li>
      <li class="contacts--item">
        <a
          target="_blank"
          href="https://hh.ru/resume/8a06b15eff0b75794d0039ed1f494d4c4b3977"
          class="big-text big--link"
          >hh.ru</a
        >
      </li>
    </ul>
  </section>
</template>

<style scoped>
.contacts {
  display: grid;
  justify-items: center;
  padding-top: 80px;
}

.contacts--list {
  display: grid;
  grid-auto-flow: column;
  gap: 15px;
  margin: 120px 0;
}

.contacts--item {
  font-family: "Noto_Sans_Mono";
  font-weight: 500;
  font-size: 1.3rem;
  line-height: 40px;
  color: var(--color-text);
}

@media (max-width: 700px) {
  .lines {
    display: none;
  }

  .contacts--list {
    grid-auto-flow: row;
    justify-items: center;
    margin-bottom: 80px;
  }
}
</style>
