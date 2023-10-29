<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode']
}
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #a17651;
  border: 1px solid #000000;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #5c3703;
  border-color: #000000;
}

.flat {
  background-color: transparent;
  color: #000000;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #edd1be;
}
</style>