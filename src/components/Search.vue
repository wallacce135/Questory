<template>
    <div id="Search">
      <input type="search" placeholder="Найти квесты">
      <input type="image" src="/img/icons/search.png">
    </div>
</template>

<style lang="scss" scoped>
    #Search {
        width: 435px;
        background: #A8ACA6;
        border-radius: 40px;
        display: flex;
        input[type=search] {
            background: #A8ACA6;
            border: none;
            height: 48px;
            padding-left: 20px;
            border-radius: 40px;
            width: calc(100% - 40px);
            color: #fff;
            font-size: 16px;
        }
        input:focus {
            outline: none;
        }
        input[type=image] {
            padding: px;
            width: 27px;
            height: 26px;
            padding: 10px;
        }
    }
</style>
