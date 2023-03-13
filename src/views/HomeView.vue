<script setup lang="ts">
function play() {
  const audio = document.querySelector("audio") as HTMLAudioElement;

  audio.play();
}
</script>

<template>
  <main class="mainContainer">
    <div class="helltcholasLogoContainer">
      <img class="helltcholas" src="/hell-tcholas.jpg" alt="imagem helltcholas">
    </div>
    <div class="helltcholasTxtContainer">
      <p>
        Helltcholas Club trata-se do grupo de alunos mais foda que já existiu nessa Fatec na turma de ADS, somos compostos por 3 integrantes, sendo um mais tcholas do que o outro.
      </p>
    </div>
    <div class="integrantes">
      <div class="integrantesTitle">
        <h1>Integrantes</h1>
      </div>
      <div class="integrantesContainer">
        <div class="integranteCard">
          <div class="integrante">
            <img src="/egrilo.jpg" alt="egrilo">
            <h1>Pathy Egrilo</h1>
          </div>
          <div class="integrantes">
            <p>
              Tanka o álcool no rolê, vê ratos na parede e apelida eles de Alves e por ai vai
            </p>
          </div>
        </div>
        <div class="integranteCard">
          <div class="integrante">
            <img src="/nerdola.jpg" alt="nerdola">
            <h1>Braia nerdola</h1>
          </div>
          <div class="integrantes">
            <p>
              Nerdola d++++, o cara usa Vue.js no Android Studio KKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKKK nem fodendo
            </p>
          </div>
        </div>
        <div class="integranteCard">
          <div class="integrante">
            <img src="/safadao.jpg" alt="safadão">
            <h1>Gabriel dark 666 true metal</h1>
          </div>
          <div class="integrantes">
            <p style="display: flex;">
              Meio <span><img style="margin: 0 10px; cursor: pointer;" @click="play();" src="/som.png" alt="">
                <audio src="/zap.mp3"></audio>
              </span> das ideia
            </p>
          </div>
        </div>
      </div>
    </div>
    <img class="capiroto" src="/capiroto.png" alt="capiroto">
  </main>
</template>

<style scoped>
.mainContainer {
  position: relative;
}
.helltcholasLogoContainer {
  width: 100%;
  display: flex;
  justify-content: center;
}
.helltcholas {
  max-width: 600px;
  width: 100%;
}
.helltcholasTxtContainer {
  padding: 0 10px;
  display: flex;
  justify-content: center;
  margin: 30px 0 0 0;
}
.helltcholasTxtContainer p {
  font-size: 2rem;
}
.capiroto {
  position: fixed;
  right: 3vw;
  bottom: 3vw;
  width: 60px;
}
.integrantes p {
  font-size: 1.6rem;
  word-wrap: break-word;
}
.integrantes p span img {
  width: 20px;
}
.integrantesTitle {
  width: 100%;
  display: flex;
  justify-content: center;
  margin: 50px 0;
}
.integrantesTitle h1 {
  font-size: 5rem;
}
.integrantesContainer {
  display: flex;
  justify-content: space-around;
  padding: 20px 0;
  flex-wrap: wrap;
}
.integrante h1 {
  font-size: 2.5rem;
  margin: 9px 0;
}
.integrante img {
  max-width: 300px;
  width: 100%;
  height: 200px;
}
.integranteCard {
  width: 300px;
  margin: 50px 10px 0 10px;
}
</style>