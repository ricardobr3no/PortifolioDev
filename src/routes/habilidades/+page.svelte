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
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut aliquam
          sed quas blanditiis laboriosam corporis, accusantium, nihil nostrum
          sunt quo ipsam voluptate. Nihil asperiores et dicta eius similique
          voluptas dolores.
        </p>
        <div class="conteudo_certificados_container">
          <h3>Meus Certificados</h3>
          <a href="/">
            <Paperclip />
            Certificados
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
    height: 100vh;
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
    max-width: 500px;
    font-family: var(--fonte-secundaria);
    font-size: 22px;
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
  .conteudo_certificados_container a {
    background-color: var(--background-color-1);
    border: solid 2px var(--fonte-color-2);
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    width: 180px;
    height: 45px;
    border-radius: 6px;
  }
  .conteudo_certificados_container a:hover {
    background-color: var(--background-color-2);
  }
  .conteudo_imagem {
    scale: 1.4;
    margin-top: 150px;
    position: relative;
  }
  .conteudo_imagem img {
    /* background-color: red; */
    border-radius: 400px;
    position: absolute;
    width: 250px;
    translate: -0px 7px;
  }
  .conteudo_imagem .circle {
    /* background-color: #b641e0;#9B53B5 */
    background-color: var(--fonte-color-2);
    border-radius: 400px;
    width: 260px;
    height: 260px;
  }
</style>
