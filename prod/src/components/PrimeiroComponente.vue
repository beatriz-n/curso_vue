<template>
<div>
     <h1>ola vue</h1>
    <p>{{ nome }} trabalho com {{ profi }}</p>
</div>
</template>

<script>
export default {
  name: 'PrimeiroComponente',
  data () {
    return {
      nome: 'beatriz',
      profi: 'programa'
    }
  }
}
</script>
