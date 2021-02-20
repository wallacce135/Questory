<template>
    <div id="Registration">
        <div class="primary-log">
            <h1>Questory</h1>
            <Logup></Logup>
        </div>
    </div>
</template>

<script>
import Logup from '.././components/Logup.vue'

export default {
  name: 'Registration',
  components: {
    Logup
  }
}
</script>

<style lang="scss">
#Registration
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
    p:hover b {
        animation: backd-go 1s forwards;
    }
    @keyframes backd-go {
        0%  {
            background: rgba(246, 163, 103, 0);
        }
        100% {
            background: rgba(246, 163, 103, 1);
        }
    }
}
</style>
