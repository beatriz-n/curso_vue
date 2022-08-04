<template>
<div>
    <p v-if="estaTrabalhando">esta trabalhando no momento</p>
    <p v-else>estou em busca de novas oportunidades</p>
    <p>utilizo as seguintes tecnologias:</p>
    <ul>
    <li v-for="(tec, index) in tecnologias" :key="index.id">{{tec}}</li>
    </ul>
    <div>
      <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrarEmail">mande uma mensagem para: {{ email }}</p>
    <p>basta clicar aqui <a v-bind:href="meuLink" target="_blank">basta clicar</a></p>
    </div>
</template>

<script>

export default {
  name: 'InfoPessoa',
  components: {},
  data () {
    return {
      estaTrabalhando: false,
      mostrarEmail: true,
      email: 'ola@gmail.com',
      meuLink: 'https://google.com',
      textoBotao: 'Mostrar email',
      tecnologias: ['javascript', 'PHP', 'VUEJS']
    }
  },
  methods: {
    showEmail () {
      this.mostrarEmail = !this.mostrarEmail
      if (!this.mostrarEmail) {
        this.textoBotao = 'textoBotao'
      } else {
        this.textoBotao = 'esconder email'
      }
    }
  }
}
</script>
