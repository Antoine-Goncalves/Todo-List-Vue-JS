<template>
  <div>
    <div class="field">
      <div class="control is-large is-loading">
        <input
          class="input is-large"
          type="text"
          placeholder="Write something.."
          :value="value"
          v-on="listeners"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["value"],
  computed: {
    listeners() {
      return {
        // Pass all component listeners directly to input
        ...this.$listeners,
        // Override input listener to work with v-model
        input: event => this.$emit("input", event.target.value)
      };
    }
  }
};
</script>

<style>
</style>