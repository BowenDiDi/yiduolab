<template>
  <button @click="handleClick" :class="buttonClass">
    <slot></slot>
  </button>
</template>
<script>
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'CustomButton',
  props: {
    type: {
      type: String,
      default: 'primary'
    },
    disabled: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    buttonClass() {
      return `custom-button custom-button-${this.type} ${this.disabled ? 'disabled' : ''}`
    }
  },
  methods: {
    handleClick() {
      if (!this.disabled) {
        this.$emit('click')
      }
    }
  }
})
</script>
<style scoped>
.custom-button {
  width: 140px;
  height: 40px;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  border-radius: 4px;
}
.custom-button-primary {
  background-color: #1688f8;
  color: white;
}
.custom-button-secondary {
  background-color: gray;
  color: white;
}
.disabled {
  cursor: not-allowed;
  opacity: 0.5;
}
</style>
