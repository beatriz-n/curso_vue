<template>
<div>
    <h2>esta é a descrição da pessoa: {{ nome }}</h2>
    <InfoPessoa></InfoPessoa>
</div>
</template>

<script>
import InfoPessoa from './InfoPessoa.vue'
export default {
  data () {
    return {
      name: 'beatriz'
    }
  },
  components: { InfoPessoa }
}
</script>
