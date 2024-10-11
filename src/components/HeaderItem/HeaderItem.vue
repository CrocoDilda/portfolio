<template>
  <header class="header container">
    <nav>
      <ul class="header--list">
        <li class="header--item">
          <a class="big-text big--link" href="#projects">Projects</a>
        </li>
        <li class="header--item">
          <a class="big-text big--link" href="#contacts">Contacts</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: end;
  align-items: center;
  max-height: 40px;
}

.header--list {
  display: flex;
  align-items: center;
  gap: 60px;
}
</style>
