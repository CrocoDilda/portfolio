<template>
  <header class="header container">
    <nav>
      <ul class="header--list">
        <li class="header--item">
          <a class="big-text header--link" href="#">Projects</a>
        </li>
        <li class="header--item">
          <a class="big-text header--link" href="#">Contact</a>
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

.header--link {
  position: relative;
  transition: 0.1s;

  &::after {
    content: "";
    position: absolute;
    width: 0%;
    height: 4px;
    background-color: var(--color-text-hover);
    bottom: -8px;
    left: 0;
    transition: 0.2s;
  }

  &:hover {
    opacity: 0.8;
    color: var(--color-text-hover);
  }

  &:hover::after {
    width: 100%;
  }
}
</style>
