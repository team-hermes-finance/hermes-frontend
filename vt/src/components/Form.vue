<template>
  <div id='par'>
    <h2>Create Your Account</h2>
    <form id='form'>
        <input class="form__input" type='text' placeholder='Email'/>
        <input class="form__input" type='text' placeholder='Username'/>
        <input class="form__input" type='password' placeholder='Password'/>
        <input class="form__input" type='password' placeholder='Confirm Password'/>
        <div class='form__submit' @click='submitForm'>
        Submit
        </div>
    </form>
  </div>
</template>

<script>
export default {
  data () {
  },
  validations: {
  },
  methods: {
    submitForm () {
      alert('Form has been submitted')
    }
  }
}
</script>

<style scoped>
#form {
    margin: 0 auto;
}
#par {
display: flex;
  justify-content: center;
  align-items: center;
}

.form__input {
  border: none;
  outline: none;
  border-bottom: 1px solid #eee;
  font-size: 1em;
  padding: 5px;
  display: flex;
  margin: 10px 0 5px 0;
}

.form__error {
  color: red;
  font-size: 0.75em;
  padding-left: 10px;
}

.form__submit {
  background-color: #0033cc;
  color: white;
  padding: 10px 20px;
  text-align: center;
  cursor: pointer;
  margin-top: 30px;
}
</style>