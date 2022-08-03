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
    </div>
</template>

<script>
export default {
  name: 'InfoPessoa',
  data () {
    return {
      estaTrabalhando: false,
      mostrarEmail: true,
      email: 'ola@gmail.com'
    }
  }
}
</script>
