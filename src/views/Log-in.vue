<template>
<div id="Login">
    <div class="primary-log">
      <h1>Questory</h1>
      <Login></Login>
      <router-link class="link" to="/auth/registration">Регистрация</router-link>
      <router-link class="link" to="/Profile">Профиль</router-link>
      <router-link class="link" to="/">Домой</router-link>
    </div>
</div>
</template>

<script>
import Login from '.././components/Login.vue'
export default {
  name: 'Log-in',
  components: {
    Login
  }
}
</script>

<style lang="scss">
  #Login {
    background-image: url('/img/greenBack.png');
    width:100%;
    height: 100vh;
    font-family: Gilroy;
    font-size: 18px;
    input + img {
    padding: 17px;
    height: 30px;
    border-radius: 0 11px 11px 0;
    background: #fff;
    }
    input:not([type=checkbox]):not([type=submit]) {
      width: calc(100% - 56.17px);
      border-radius: 11px 0 0 11px;
    }
  }
  .log-form {
    p {
      margin-bottom: 25px;
      font-weight: 500;
      color: #464845;
      display: flex;
    }
    input:not([type=checkbox]):not([type=submit]) {
      padding:20px;
      border: none;
      box-shadow: 0px 4px 10px rgba(130, 127, 127, 0.25);
      font-size: 20px;
      font-family: 'Comfortaa';
      color: #64AA43;
    }
    input::placeholder {
      color: #9ED186;
    }
    input,
    input:focus,
    input:active {
      outline: none;
      align-items: baseline;
    }
    .checkbox-type {
      display: flex;
      input[type=checkbox] {
        display: none;
      }
      input[type=checkbox]:checked + label::before {
        content: "\2714";
        color: #F6A367;
        font-size: 35px;
        text-align: center;
        line-height: 35px;
      }
      label {
        cursor: pointer;
        display: flex;
      }
      label::before {
        content: "";
        display: block;
        // display: inline-block;
        // vertical-align: middle;
        width: 35px;
        height: 35px;
        background: #FFFFFF;
        box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.12);
        border-radius: 5px;
        margin-right: 16px;
        cursor: pointer;
      }
    }
    input[type=submit] {
      width: 100%;
      padding: 20px;
      font-size: 16px;
      font-weight: bold;
      border: #64AA43 4px solid;
      color: #64AA43;
      border-radius: 40px;
      background: rgba(0, 0, 0, 0);
    }
    input:invalid, input:required {
      border: #F24848 2px solid;
    }
  }
  .primary-log {
    width: 400px;
    margin: 0 auto;
    padding-top: 16vh;
  }
  h1 {
    color: #fff;
    font-size: 96px;
    margin-bottom: 60px;
    text-align: center;
  }
  a {
    text-align: right;
    text-decoration: underline;
  }
</style>
