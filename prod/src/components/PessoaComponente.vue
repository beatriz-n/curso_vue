<template>
<div>
    <h2></h2>
    <InfoPessoa :email="email"/>
    <FormComponente></FormComponente>
</div>
</template>

<script>
import InfoPessoa from './InfoPessoa.vue'
import FormComponente from './FormComponente.vue'
export default {
  data () {
    return {
      name: 'beatriz',
      email: 'assdasd@asdsd.com'
    }
  },
  components: { InfoPessoa, FormComponente }
}
</script>
