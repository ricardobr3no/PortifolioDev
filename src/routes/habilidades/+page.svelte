<script>
  import Header from "../../components/Header.svelte";
  import Footer from "../../components/Footer.svelte";
  import { Paperclip } from "lucide-svelte";
  import foto from "../../assets/include4.png";
</script>

<div class="background">
  <Header />
  <main>
    <div class="conteudo">
      <div class="conteudo_paragrafos">
        <h1>
          Minhas <span style="color:var(--fonte-color-2)">Habilidades</span>
        </h1>
        <ul>
          <li>Desenvolvedor backend pelo INOVA MARANHÃO</li>
          <li>Graduando de C&T na UFMA</li>
          <li>Tecnico em Eletrônica no IFMA</li>
          <!-- <li>Tecnico em eletronica pelo IFMA</li> -->
        </ul>

        <div class="conteudo_certificados_container">
          <h3>Meus Certificados</h3>
          <a href="/">
            <Paperclip />
            <span>Certificados</span>
          </a>
        </div>
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
    text-decoration: none;
  }
  .background {
    z-index: -10;
    background-color: var(--background-color-1);
    background-blend-mode: color;
  }
  main {
    opacity: 1;
    min-height: 100vh;
    /* margin: 50px; */
    justify-content: space-around;
  }
  .conteudo {
    display: flex;
    justify-content: space-around;
    /* background-color: #5b4d61; */
    color: var(--fonte-color-1);
    align-items: center;
    border-radius: 12px;
  }
  .conteudo_paragrafos {
    max-width: 37.5rem;
    font-family: var(--fonte-secundaria);
    font-size: 1.4rem;
  }
  .conteudo_paragrafos h1 {
    font-family: var(--fonte-primaria);
    /* font-size: 40px; */
  }
  .conteudo_certificados_container {
    width: 80%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .conteudo_certificados_container span {
    margin-left: 0.625rem;
  }
  .conteudo_certificados_container a {
    background-color: var(--background-color-1);
    border: solid 2px var(--fonte-color-2);
    display: flex;
    align-items: center;
    justify-content: center;
    width: 11.25rem;
    height: 3rem;
    border-radius: 6px;
  }
  .conteudo_certificados_container a:hover {
    background-color: var(--background-color-2);
  }
  .conteudo_imagem {
    scale: 1.4;
    margin-top: 9.4rem;
    position: relative;
    margin-bottom: 5rem;
    margin-top: 5rem;
  }
  .conteudo_imagem img {
    /* background-color: red; */
    border-radius: 50rem;
    position: absolute;
    width: 15.6rem;
    translate: -0px 0.45rem;
  }
  .conteudo_imagem .circle {
    /* background-color: #b641e0;#9B53B5 */
    background-color: var(--fonte-color-2);
    border-radius: 25rem;
    width: 16.25rem;
    height: 16.25rem;
  }
  /* responsividade */
  @media (max-width: 56rem) {
    .conteudo {
      flex-direction: column-reverse;
      flex-grow: 1;
    }
    h1 {
      text-align: center;
    }
    .conteudo_imagem {
      scale: 1;
    }

    .conteudo_certificados_container {
      width: 100%;
    }
    .conteudo_certificados_container a {
      height: 4.4rem;
      width: 60%;
    }
  }
</style>
