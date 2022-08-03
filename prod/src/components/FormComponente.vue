<template>
<form action="">
    <InputText></InputText>
    <br>
    <InputText></InputText>
    <SubmitForm></SubmitForm>
</form>
</template>

<script>
import InputText from './form/InputText.vue'
import SubmitForm from './form/SubmitForm.vue'

export default {
  name: 'FormComponent',
  components: { InputText, SubmitForm }
}
</script>
