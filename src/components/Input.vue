<template>
  <div>
    <input type="text" :value="msg" @input="changeMessage" />
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  props: ["msg"],
  data() {
    return {
      message: ""
    };
  },
  methods: {
    changeMessage(event) {
      this.message = event.target.value;
      // this emits our message after we set it to the target value of the method executed.
      this.$emit("messageChanged", this.message);
    }
  }
};
</script>
