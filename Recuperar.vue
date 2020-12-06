<template>
  <view class="container">
    <status-bar background-color="black" bar-style="light-content" />
    <text class="text-login">Recuperar</text>
    <text class="label">E-mail</text>
    <text-input class="input"/>
    <view class="itens"> 
      <button class="btn-entrar" title="Enviar" color="black" :on-press="pressionar">
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      email: "E-mail",
      senha: "Senha",
    };
  },
  methods: {
    pressionar: function () {
      alert("Olá, usuário!");
    },
  },
};
</script>

<style>
.container {
  background-color: white;
  align-items: center;
  display: flex;
}

.itens {
  display: flex;
}

.recuperar {
  align-self: flex-start;
  margin: 15px 10px;
}

.label {
  align-self: flex-start;
}
.text-login {
  margin: 30%;
  font-size: 40px;
  color: black;
}

.input {
  width: 98%;
  margin: 10px 10px;
  border-radius: 1px;
  padding: 10px;
  border-width: 1;
}
</style>
