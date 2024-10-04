<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import Redes from "../components/Redes.svelte";
  import foto from "../assets/greyhound-dog-with-towel-after-bath.jpg";
</script>

<div class="background">
  <Header />
  <main>
    <div class="conteudo">
      <div class="conteudo_paragrafos">
        <h1>Ricardo <span style="color:var(--fonte-color-2)">Breno</span></h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut aliquam
          sed quas blanditiis laboriosam corporis, accusantium, nihil nostrum
          sunt quo ipsam voluptate. Nihil asperiores et dicta eius similique
          voluptas dolores.
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut aliquam
          sed quas blanditiis laboriosam corporis, accusantium, nihil nostrum
          sunt quo ipsam voluptate. Nihil asperiores et dicta eius similique
          voluptas dolores.
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
  main {
    opacity: 1;
    height: 100vh;
    /* justify-content: space-around; */
  }
  .conteudo {
    display: flex;
    justify-content: space-around;
    /* margin-left: 50px; */
    /* margin-right: 150px; */
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
  .conteudo_imagem {
    scale: 1.4;
    margin-top: 50px;
    position: relative;
  }
  .conteudo_imagem img {
    background-color: red;
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
