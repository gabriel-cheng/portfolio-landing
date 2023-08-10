<script setup lang="ts"></script>

<template>
    <footer id="contatos">
        <div class="contatos-subcontainer">
            <div class="contatos-title">
                <h1>Contatos</h1>
            </div>
            <div class="contatos-icons">
                <a href="mailto:gabriel_carvalho.contato@outlook.com">
                    <div class="box-contato contato-email">
                        <div class="contato-icon">
                            <img src="/icons/email-purple.png" alt="">
                        </div>
                        <div class="contato-icon-title">
                            <h1>E-mail</h1>
                        </div>
                        <div class="contato-icon-access">
                            <p>gabriel_carvalho.contato@outlook.com</p>
                        </div>
                    </div>
                </a>
                <a href="https://wa.me/5518991163599?text=Ol%C3%A1+Gabriel%2C+tudo+bem%3F+Estou+entrando+em+contato+com+voc%C3%AA+atrav%C3%A9s+do+seu+portf%C3%B3lio%2C+podemos+conversar+quando+voc%C3%AA+estiver+dispon%C3%ADvel%3F">
                    <div class="box-contato contato-telefone">
                        <div class="contato-icon">
                            <img src="/icons/whatsapp-purple.png" alt="">
                        </div>
                        <div class="contato-icon-title">
                            <h1>Contato/whatsapp</h1>
                        </div>
                        <div class="contato-icon-access">
                            <p>+55(18)99116-3599</p>
                        </div>
                    </div>
                </a>
                <a href="https://linkedin.com/in/gabriel-henrique-ita">
                    <div class="box-contato contato-linkedin">
                        <div class="contato-icon">
                            <img src="/icons/linkedin-purple.png" alt="">
                        </div>
                        <div class="contato-icon-title">
                            <h1>Linkedin</h1>
                        </div>
                        <div class="contato-icon-access">
                            <p>@/in/gabriel-henrique-ita</p>
                        </div>
                    </div>
                </a>
                <a href="https://github.com/gabriel-cheng">
                    <div class="box-contato contato-github">
                        <div class="contato-icon">
                            <img src="/icons/github-purple.png" alt="">
                        </div>
                        <div class="contato-icon-title">
                            <h1>Github</h1>
                        </div>
                        <div class="contato-icon-access">
                            <p>@/gabriel-cheng</p>
                        </div>
                    </div>
                </a>
            </div>
        </div>
    </footer>
</template>

<style scoped>
#contatos {
    width: 100%;
    margin: 90px 0 0 0;
    display: flex;
    justify-content: center;
}
.contatos-subcontainer {
    display: flex;
    flex-direction: column;
    padding: 0 0 20px 0;
}
.contatos-title {
    text-align: center;
    margin: 0 0 80px 0;
}
.contatos-title > h1 {
    font-size: 4rem;
    color: #fff;
}
.contatos-icons {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 90px;
    padding: 0 20px;
}
.contato-icon-title > h1 {
    font-size: 1.9rem;
    color: #fff;
}
.contato-icon > img {
    max-width: 60px;
}
.contato-icon-access > p {
    font-size: 1.5rem;
    color: #c4c4c4;
}
.box-contato {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
    transition: 0.2s ease-in-out;
}
.box-contato:hover {
    cursor: pointer;
    transform: scale(1.1);
    transition: 0.2s ease-in-out;
}
</style>