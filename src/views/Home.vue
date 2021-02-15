<template>
  <div class="home">
    <div class="primary-log">
      <h1>Questory</h1>
      <form class="log-form">
        <p><input placeholder="Логин"><img src="/img/icons/person.png"></p>
        <p><input placeholder="Пароль"><img src="/img/icons/lock.png"></p>
        <p><input type="checkbox"><label>Запомнить меня</label></p>
        <p><input type="submit" value="Войти"></p>
      </form>
      <router-link class="link" to="/about">Регистрация</router-link>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss">
  .home {
    background-image: url('/img/greenBack.png');
    width:100%;
    height: 100vh;
    font-family: Gilroy;
    font-size: 18px;
  }
  .log-form {
    p {
      margin-bottom: 25px;
      font-weight: 500;
      color: #464845;
      display: flex;
    }
    input:not([type="checkbox"]):not([type="submit"]) {
      padding:20px;
      width: calc(100% - 56.17px);
      border-radius: 11px 0 0 11px;
      border: none;
      box-shadow: 0 4px 10px rgba(130, 127, 127, 0.25);
      font-size: 20px;
      font-family: 'Comfortaa';
    }
    input::placeholder {
      color: #9ED186;
    }
    input,
    input:focus,
    input:active {
      outline: none;
    }
    input[type="checkbox"] {
      display: none;
    }
    input[type="submit"] {
      width: 100%;
      padding: 20px;
      font-size: 16px;
      font-weight: bold;
      border: #64AA43 4px solid;
      color: #64AA43;
      border-radius: 40px;
      background: rgba(0, 0, 0, 0);
    }
    label::before {
      content: '';
      width: 35px;
      height: 35px;
      background: #FFF;
      box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.12);
      border-radius: 5px;
      margin: 0px 13px;
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
  img {
    padding: 17px;
    height: 30px;
    border-radius: 0 11px 11px 0;
    background: #fff;
  }
  a {
    text-align: right;
    text-decoration: underline;
  }
</style>
