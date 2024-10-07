<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import Redes from "../components/Redes.svelte";
  import foto from "../assets/minhaFoto.jpeg";
</script>

<div class="background">
  <Header />
  <main>
    <div class="conteudo">
      <div class="conteudo_paragrafos">
        <h1>Ricardo <span style="color:var(--fonte-color-2)">Aguiar</span></h1>
        <p>
          Olá! Sou desenvolvedor backend e graduando em C&T, apaixonado por
          tecnologia e sempre em busca de novos desafios. Tenho experiência em
          diversas tecnologias, incluindo Python, C, Node.js e MySQL.
        </p>
        <p>
          Meu objetivo é contribuir para projetos inovadores e desafiadores,
          ajudando a criar soluções eficientes e escaláveis que impactem
          positivamente a vida das pessoas.
        </p>
        <Redes />
      </div>
      <div class="conteudo_imagem">
        <img src={foto} alt="minha foto" />
        <div class="circle"></div>
      </div>
    </div>
  </main>
  <Footer />
</div>

<style>
  :root {
    @import url("https://fonts.googleapis.com/css2?family=Do+Hyeon&family=Lato&display=swap");

    --background-color-1: #332d36;
    --background-color-2: #2f2333;
    --cor-secundaria: #7e578c;
    --fonte-color-1: white;
    --fonte-color-2: #9b53b5;

    --fonte-primaria: "Do Hyeon", sans-serif;
    --fonte-secundaria: "Lato", sans-serif;
  }
  * {
    color: white;
    font-style: normal;
  }
  .background {
    z-index: -10;
    background-color: var(--background-color-1);
    background-blend-mode: color;
  }
  p {
    text-align: start;
  }
  main {
    opacity: 1;
    min-height: 100vh;
    /* justify-content: space-around; */
  }
  .conteudo {
    display: flex;
    justify-content: space-around;
    flex-grow: 1;
    /* margin-left: 3.125rem; */
    /* margin-right: 150px; */
    /* background-color: #5b4d61; */
    color: var(--fonte-color-1);
    align-items: center;
    border-radius: 12px;
  }
  .conteudo_paragrafos {
    max-width: 38rem;
    font-family: var(--fonte-secundaria);
    font-size: 1.5rem;
  }
  .conteudo_paragrafos h1 {
    font-family: var(--fonte-primaria);
    /* font-size: 40px; */
  }
  .conteudo_imagem {
    scale: 1.4;
    margin-top: 3.125rem;
    margin-bottom: 3.125rem;
    position: relative;
  }
  .conteudo_imagem img {
    /* background-color: red; */
    border-radius: 400px;
    position: absolute;
    width: 15.625rem;
    translate: -0px 7px;
  }
  .conteudo_imagem .circle {
    /* background-color: #b641e0;#9B53B5 */
    background-color: var(--fonte-color-2);
    border-radius: 400px;
    width: 16.25rem;
    height: 16.25rem;
  }
  /* responsividade */
  @media (max-width: 56rem) {
    .conteudo {
      flex-direction: column-reverse;
    }

    h1 {
      text-align: center;
    }
    .conteudo_paragrafos p {
      padding-left: 7%;
      padding-right: 5%;
    }
    .conteudo_imagem {
      scale: 1;
    }
  }
</style>
