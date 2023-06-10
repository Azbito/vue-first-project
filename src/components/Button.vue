<template>
  <button @title="title">{{text}}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
  },
  methods: {
    title: String,
  }
};
</script>

<style lang="scss">
button {
  background-color: rgb(165, 29, 219);
  border: none;
  outline: none;
  color: white;
  padding: .5rem;
  border-radius: .5rem;
  transition: .2s;
  cursor: pointer;

  &:hover {
    background-color: rgb(183, 0, 255);
  }

  &:active {
    background-color: rgb(113, 21, 150);
  }
}
</style>