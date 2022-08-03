<template>
<div>
    <p v-if="estaTrabalhando">esta trabalhando no momento</p>
    <p v-else>estou em busca de novas oportunidades</p>
    <p>utilizo as seguintes tecnologias:</p>
    <ul>
        <li>JavaScript</li>
        <li>PHP</li>
        <li>VUEJS</li>
    </ul>
    <p v-show="mostrarEmail">mande uma mensagem para: {{ email }}</p>
    <p>basta clicar aqui <a v-bind:href="meuLink" target="_blank">basta clicar</a></p>
    <PictureComponente></PictureComponente>
    </div>
</template>

<script>
import PictureComponente from './form/pictureComponente.vue'
export default {
  name: 'InfoPessoa',
  data () {
    return {
      estaTrabalhando: false,
      mostrarEmail: true,
      email: 'ola@gmail.com',
      meuLink: 'https://google.com'
    }
  },
  components: { PictureComponente }
}
</script>
