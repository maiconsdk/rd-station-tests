<script lang="ts" setup>

const handleSubmit = ({currentTarget}: Event) => {
  const form = currentTarget as HTMLFormElement
  const formData = new FormData(form)

  console.log(formData)
}
</script>
<template>
  <div class="container">
    <form class="form" action="/" @submit="handleSubmit">
      <label class="form__label" for="fullname">
        <input class="form__input" type="text" name="fullname" id="fullname" placeholder="Digite o seu nome completo" required>
      </label>
  
      <label class="form__label" for="email">
        <input class="form__input" type="email" name="email" id="email" placeholder="Digite o seu e-mail corporativo">
      </label>
  
      <label class="form__label" for="companyName">
        <input class="form__input" type="text" name="companyName" id="companyName" placeholder="Digite nome da empresa">
      </label>
  
      <label class="form__label" for="phone">
        <input class="form__input" type="tel" name="phone" id="phone" placeholder="Digite o seu telefone">
      </label>
  
      <label class="form__label" for="employessCount">
        <input class="form__input" type="tel" name="employessCount" id="employessCount" placeholder="Digite o número de funcionários">
      </label>
  
      <label class="form__label" for="role">
        <input class="form__input" type="tel" name="role" id="role" placeholder="Digite o seu cargo">
      </label>
  
      <button type="submit">Enviar</button>
    </form>
  </div>
</template>
<style lang="css" scoped>
.container {
  margin: 0 auto;
}

.form {
  display: flex;
  flex-direction: column;
  gap: .5rem;
}
</style>