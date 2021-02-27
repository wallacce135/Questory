<template>
    <div class="dark-layer">
        <section>
            <div>
                <img class="turb" src="/img/greenBack.png">
            </div>
            <div>
                <article>
                    <div class="btn-close"><img class="close-pop" src="/img/icons/close.png"></div>
                    <h2>Квест1</h2>
                    <div class="description">
                        <p>Описание квеста1 шикарное, классное и самое лучшее. Описания лучше вы никогда не найдете.</p>
                        <b><u><a>Краеведческая экскурсия</a></u></b>
                    </div>
                    <div class="timer">
                        <img src="/img/icons/time.png">
                        <span>2ч 0мин</span>
                    </div>
                </article>
            </div>
        </section>
    </div>
</template>

<style lang="scss" scoped>
    .dark-layer {
        width: 100%;
        height: 100vh;
        overflow: hidden;
        background: rgba(0, 0, 0, 0.63);
        position: absolute;
        top: 0;
        left: 0;
        section {
            width: 890px;
            display: flex;
            background: #FFFFFF;
            box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.07);
            border-radius: 11px;
            padding: 20px;
            margin: 15vh auto;
        }
        section > div {
            width: 50%;
            height: 368px;
            overflow: hidden;
            .turb {
                height: 100%;
                padding: 0 !important;
            }
            .btn-close {
                width: 100%;
                text-align: right;
                img {
                    width: 30px;
                    height: 30px;
                    padding: 0;
                }
            }
        }
        article {
            h2, .description {
                margin-bottom: 36px;
            }
            .timer {
                display: flex;
                img {
                    width: 26px !important;
                    height: 26px;
                    padding: 0 13px 0 0 !important;
                }
            }
        }
    }
</style>
