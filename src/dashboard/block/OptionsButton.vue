<template>
  <div class="options-button">
    <img
      src="/img/settings.svg"
      @click="options"
    >
  </div>
</template>

<script>
export default {
  name: 'OptionsButton',
  props: {
    onClick: Function
  },
  methods: {
    options: function() {
      this.onClick();
    }
  }
}
</script>

<style scoped>
.options-button {
  position: absolute;
  top: 0;
  right: 0;

  display: none;
}

article:hover .options-button {
  cursor: pointer;
  display: block;
}

img {
  width: 1.5rem;
  height: 1.5rem;
  background: rgb(255, 255, 255, 75%);
  border-radius: 1.5rem;
  padding: 5px;
}
</style>
