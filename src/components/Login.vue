<template>
  <section>
    <form v-on:submit.prevent="onSubmit">
      <div>
        <label>Email</label>
        <input type = "text" placeholder = "user@example.com"/>
      </div>
      <div>
        <label>Password</label>
        <input :type = "inputType" placeholder = ""/>
        <button v-on:click="togglePasswordField" class = "toggle-btn" type = "button">Show</button>
      </div>
      <div>
        <button type = "submit">Login</button>
      </div>
    </form>
  </section>
</template>

<script>
export default {
  name: 'Login',
  data: function() {
    return {
      inputType: 'password'
    }
  },
  props: {
  },
  methods: {
    onSubmit: function(e) {
      this.togglePasswordField();
    },
    togglePasswordField: function() {
      this.inputType = this.inputType === 'password' ? 'text' : 'password';
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang = "scss" scoped>
section {
  display: flex;
  justify-content: center;
  align-items: center;
  height: calc(100vh - 50px);
  form {
    width: 80%;
    max-width: 480px;
  }
  div {
    position: relative;
    margin: 2rem 0;
    text-align: left;
  }
  .toggle-btn {
    position: absolute;
    right: 0; 
    background-color: transparent;
    border: none;
    font-weight: bold;
    text-transform: uppercase;
  }
  label {
    display: block;
    font-size: 1rem;
    font-weight: bold;
  }
  input {
    width: 100%;
    border-left: none;
    border-right: none;
    border-top: none;
    border-bottom: 1px solid #2c3e50;
    padding: 0.5rem 0rem;
    font-size: 1rem;
  }

}
</style>
