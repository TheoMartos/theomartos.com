<template>
  <b-container>
    <h4 class="text-center">Contact me</h4>
    <b-form @submit="onSubmit">
      <b-form-group id="email-input-group" label="Email address:" label-for="email-email-input">
        <b-form-input id="email-email-input" v-model="form.email" type="email" placeholder="Enter your email" required>
        </b-form-input>
      </b-form-group>

      <b-form-group id="message-input-group" label="Enter your message:" label-for="message-email-input">
        <b-form-textarea id="message-email-input" v-model="form.message" placeholder="2000 caracters max" rows="7" @keyup="checkMessageLength" required>
        </b-form-textarea>
      </b-form-group>
      <b-button type="submit" block variant="secondary">Submit</b-button>
    </b-form>
  </b-container>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          email: '',
          message: ''
        },
      }
    },
    methods: {
      onSubmit(evt) {
        evt.preventDefault()
        alert(JSON.stringify(this.form))
      },
      checkMessageLength(evt) {
        if (this.form.message.length > 2000)
          this.form.message = this.form.message.substring(0, 1999)
      }
    }
  }

</script>
