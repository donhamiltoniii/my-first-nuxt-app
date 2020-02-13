<template>
  <div>
    <h1>All users!</h1>
    <div>
      <input type="text" v-model="id" />
      <button @click="onLoadUser">Smack that button</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: ""
    };
  },
  methods: {
    onLoadUser() {
      this.$router.push(`/users/${this.id}`);
    }
  }
};
</script>
