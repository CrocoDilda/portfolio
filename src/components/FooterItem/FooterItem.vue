<template>
  <footer class="footer">
    <p class="footer--text">
      Developer by
      <a
        href="https://github.com/CrocoDilda"
        target="_blank"
        class="footer--link"
        >CrocoDilda</a
      >
    </p>
  </footer>
</template>

<style scoped>
.footer {
  display: flex;
  justify-content: center;
  padding: 30px 0;
}

.footer--text {
  color: var(--color-text);
}

.footer--link {
  color: var(--color-terminal-link);
  transition: color 0.2s;

  &:hover {
    color: var(--color-terminal-link-hover);
  }
}
</style>
