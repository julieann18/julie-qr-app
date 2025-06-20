<template>
  <v-container class="fill-height d-flex align-center justify-center">
    <v-card class="pa-5" width="400">
      <v-card-title class="justify-center">Sign In Page</v-card-title>

      <v-card-text>
        <v-text-field label="Email" v-model="email" type="email" outlined dense></v-text-field>
        <v-text-field label="Password" v-model="password" type="password" outlined dense></v-text-field>
      </v-card-text>

      <v-card-actions class="justify-center">
        <v-btn color="primary" @click="signIn">Sign In</v-btn>
      </v-card-actions>
    </v-card>
  </v-container>
</template>

<script>
export default {
  layout: 'auth',
  data() {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    signIn() {
    
      console.log('Signing in with', this.email, this.password)
    }
  }
}
</script>
