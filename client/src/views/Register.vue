<template>
  <v-container>
    <v-layout row wrap>
      <v-flex xs6 offset-xs3>
        <h1>Register</h1>
        <v-text-field label="Email" placeholder="Email"></v-text-field>
        <v-text-field label="Password" placeholder="Password" type="password" autocomplete="new-password"></v-text-field>
        <v-btn color="green" dark>
          <v-icon>account_circle</v-icon>
          Register
        </v-btn>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    name: 'Register',
  };
</script>

<style scoped>

</style>
