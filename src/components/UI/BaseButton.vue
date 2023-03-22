<template>
  <button :type="type" :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['type', 'mode']
}
</script>
<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #c89300;
  border: 1px solid #c89300;
  border-radius: 5px;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #a67a01;
  border-color: #a67a01;
}

.flat {
  background-color: transparent;
  color: #e7b45e;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #f5d1a5;
  border-radius: 5px;
}
</style>