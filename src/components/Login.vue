<template>
    <form class="log-form" id="log" @submit.prevent="login">
        <p><input required placeholder="Логин" type="text" v-model="login"><img src="/img/icons/person.png"></p>
        <p><input required placeholder="Пароль" type="password" v-model="password"><img src="/img/icons/lock.png"></p>
        <p class="checkbox-type" ><input id="remember" type="checkbox"><label for="remember" style="user-select:none">Запомнить меня</label></p>
        <p><input type="submit" value="Войти"></p>
    </form>
</template>

<script>
export default {}
</script>
