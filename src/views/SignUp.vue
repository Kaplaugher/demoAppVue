<template>
    <form class='form-container' @submit.prevent="signUp">
        <b-field label="Name">
            <b-input v-model="user.name" placeholder="Name"></b-input>
        </b-field>

        <b-field label="Email">
            <b-input v-model="user.email" type="email" placeholder="Email" >
            </b-input>
        </b-field>

        <b-field label="Username">
            <b-input v-model="user.username" type="text" placeholder="Username"></b-input>
        </b-field>

        <b-field label="Password">
            <b-input v-model="user.password" type="password" placeholder="Password" password-reveal>
            </b-input>
        </b-field>

        <button class="button is-link" type="submit">Sign Up</button>
    </form>
</template>

<script>
export default {
  name: "signUp",
  data: () => ({
    user: {
      name: "",
      email: "",
      username: "",
      password: "",
    }
  }),
  methods: {
      signUp() {
        console.log('helooooo')
      }
  }
};
</script>

<style <style lang="scss" scoped>
.field {
  width: 300px;
}
.form-container {
  display: grid;
  justify-content: center;
}
</style>
