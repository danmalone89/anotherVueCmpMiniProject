<template>
  <div>
    <p>
      This mini-project shows how communication occurs between a child (input)
      and parent (message) component.
    </p>
    <app-message></app-message>
  </div>
</template>

<script>
import Message from "./components/Message.vue";
import Input from "./components/Input.vue";
export default {
  name: "App",
  components: {
    appMessage: Message,
    appInput: Input
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
