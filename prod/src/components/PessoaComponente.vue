<template>
<div>
    <h2></h2>
    <InfoPessoa></InfoPessoa>
    <FormComponente></FormComponente>
</div>
</template>

<script>
import InfoPessoa from './InfoPessoa.vue'
import FormComponente from './FormComponente.vue'
export default {
  data () {
    return {
      name: 'beatriz'
    }
  },
  components: { InfoPessoa, FormComponente }
}
</script>
