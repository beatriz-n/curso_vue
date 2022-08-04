<template>
<div>
  <HeaderScoped></HeaderScoped>
  <PrimeiroComponente/>
  <LifeCycle></LifeCycle>
  <PessoaComponente></PessoaComponente>
  <p>formulario usando hierarquia de componentes</p>
</div>

</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import PessoaComponente from './components/PessoaComponente.vue'
import HeaderScoped from './components/headerScoped.vue'

export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    PessoaComponente,
    HeaderScoped
  }
}
</script>

<style>
body{
  background-color: black;
  color: aliceblue;
}

a{
  color: red;
}
</style>
