<script setup lang="ts">
</script>

<template>
    <section id="inicio">
        <div class="section-1-subcontainer">
          <div class="name-container">
            <p>Gabriel Carvalho,</p>
          </div>
          <div class="profission-container">
            <p>Desenvolvedor Web</p>
          </div>
          <div class="buttons-container">
            <div class="">
              <a href="/">
                <button class="section-1-btn btn-1">Baixar currículo</button>
              </a>
            </div>
            <div class="">
              <a href="https://wa.me/5518991163599?text=Ol%C3%A1+Gabriel%2C+tudo+bem%3F+Estou+entrando+em+contato+com+voc%C3%AA+atrav%C3%A9s+do+seu+portf%C3%B3lio%2C+podemos+conversar+quando+voc%C3%AA+estiver+dispon%C3%ADvel%3F">
                <button class="section-1-btn btn-2">Entrar em contato</button>
              </a>
            </div>
          </div>
        </div>
        <div class="section-1-image">
          <div>
            <a href="https://github.com/gabriel-cheng" target="_blank">
              <img class="image" src="/padrao-perfil.png" alt="imagem de perfil">
            </a>
          </div>
        </div>
    </section>
</template>

<style scoped>
#inicio {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  align-items: center;
  margin: 90px 0 0 0;
}
.name-container p {
  color: #fff;
  font-size: 5rem;
}
.image {
  max-width: 420px;
  width: 100%;
  border-radius: 50%;
  border: 3px solid var(--purple-background);
  transition: 0.2s ease-in-out;
}
.image:hover {
  transform: scale(1.1);
  transition: 0.2s ease-in-out;
}
.profission-container {
  font-size: 9rem;
  color: var(--purple-background);
}
.buttons-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 20px 0 0 0;
}
.section-1-btn {
  width: 210px;
  font-size: 1.6rem;
  height: 40px;
  border-radius: 20px;
  outline: none;
  border: none;
  cursor: pointer;
  color: #fff;
  border: 1px solid #fff;
  transition: 0.3s ease-in-out;
}
.btn-1 {
  background-color: var(--purple-background);
}
.btn-1:hover {
  background-color: var(--purple-background-2);
  transition: 0.3s ease-in-out;
  transform: scale(1.1);
}
.btn-2 {
  background-color: transparent;
}
.btn-2:hover {
  transform: scale(1.1);
  background-color: #fff;
  color: #000;
}
@media screen and (max-width: 990px) {
  #inicio {
    flex-direction: column-reverse;
    margin: 40px 0 0 0;
  }
  .name-container,
  .profission-container {
    padding: 0 20px;
  }
  .buttons-container {
    justify-content: center;
  }
  .section-1-image {
    padding: 0 10px;
  }
}
@media screen and (max-width: 480px) {
  .name-container p {
    font-size: 12vw;
  }
  .profission-container p {
    font-size: 12vw;
  }
  .section-1-btn {
    width: 90vw;
    height: 60px;
    border-radius: 40px;
  }
}
</style>