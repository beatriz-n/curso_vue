<template>
<form action="" @submit="enviarForm($event)">
    <input type="text" v-model="name">
    <br>
    <input type="text" v-model="email">
    <SubmitForm></SubmitForm>
</form>
</template>

<script>
import SubmitForm from './form/SubmitForm.vue'

export default {
  name: 'FormComponent',
  components: { SubmitForm },
  data () {
    return {
      name: '',
      email: ''
    }
  },
  methods: {
    enviarForm (e) {
      e.preventDefault()
      const name = this.name
      const email = this.email
      console.log('funcionou')
      console.log('o nome é: ' + name)
      console.log('o email é: ' + email)
    }
  }
}
</script>

<style scoped>
p{
  margin: 150px;
}
</style>
