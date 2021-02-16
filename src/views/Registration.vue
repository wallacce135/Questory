<template>
    <div class="Registration">
        <div class="primary-log">
            <h1>Questory</h1>
            <form action="" class="log-form">
                <p><input type="text" placeholder="Имя"></p>
                <p><input type="text" placeholder="Фамилия"></p>
                <p><input type="text" placeholder="Отчество"></p>
                <p><input type="date" placeholder="Дата рождения"></p>
                <p><input type="text" placeholder="Ник"></p>
                <p><input type="email" placeholder="Эл. почта"></p>
                <p><input type="password" placeholder="Пароль"></p>
                <p><input type="password" placeholder="Повторите пароль"></p>
                <p><input type="submit" value="Зарегистироваться"></p>
            </form>
        </div>
    </div>
</template>

<style lang="scss">
.Registration
{
    font-family: Gilroy;
    background: linear-gradient(118.61deg, #64AA43 -20.89%, rgba(100, 170, 67, 0) 67.65%), linear-gradient(222.28deg, #9ED186 23.81%, rgba(158, 209, 134, 0) 92.86%), #ACDF9B;
    width: 100%;
    padding-bottom: 50px;
    // height: 100vh;
    p > input {
        border-radius: 11px;
        width: 100%;
    }
}
</style>
