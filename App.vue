<template>
  <view class="container">
    <status-bar background-color="black" bar-style="light-content" />
    <text class="text-login">Login</text>
    <text-input class="input" />
    <text-input class="input" />
    <text class="avisos2">Esqueceu a senha?</text>
    <button class="btn-entrar" title="Login" color="black" :on-press="pressionar">
  </view>
</template>

<script>
import { Button } from 'react-native';
export default {
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


.avisos{
  padding: 10px;
  align-items: flex-end;
}
.text-login {
  font-size: 40px;
  color: black;
}

.input {
  width: 90%;
  margin: 10px 10px;
  border-radius: 1px;
  padding: 10px;
  border-width: 1;
}
</style>
