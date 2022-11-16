<template>
  <div>
    <span> this is custom input component {{ number }}</span>
    <input v-model="username" type="text" />
    <span :title="spanTitle">{{ username }}</span>
  </div>
</template>

<script>
export default {
  name: "InputComponent",
  data() {
    return {
      username: "",
      spanTitle: "username is here",
    };
  },
  props: ["number"],
};
</script>

<style>
</style>