<script>
  import Header from "../../components/Header.svelte";
  import Footer from "../../components/Footer.svelte";
  import Card from "../../components/Card.svelte";

  import imagemExploraMaranhao from "../../assets/screencapture-desafio-v-explora-maranhao-vercel-app-2024-10-05-19_00_46.png";
  import imagemShooter2D from "../../assets/pygame.png";
</script>

<div class="background">
  <Header />
  <main>
    <div class="conteudo">
      <div class="conteudo_paragrafos">
        <h1>
          Meus <span style="color:var(--fonte-color-2)">Projetos</span>
        </h1>
        <p>
          Desenvolvedor backend com forte base em JavaScript e Python. Atuo no
          desenvolvimento de APIs RESTful e integração de sistemas. Abaixo,
          apresento alguns dos projetos que contribui ativamente.
        </p>
      </div>
      <div class="conteudo_projetos">
        <Card
          title="explora-maranhão"
          imageUrl={imagemExploraMaranhao}
          source="https://github.com/kauanguilhermesantos/desafio-v-explora-maranhao"
        />
        <Card
          title="shooter2D-pygame"
          imageUrl={imagemShooter2D}
          source="https://github.com/ricardobr3no/space-shooter-pygame"
        />
        <!-- <Card /> -->
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
    --cor-auxiliar: #5b4d61;
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
    min-height: 100vh;
    /* margin-left: 150px; */
    /* margin-right: 150px; */
    /* justify-content: space-around; */
  }
  .conteudo {
    display: flex;
    flex-direction: column;
    /* justify-content: space-around; */
    /* margin: 50px; */
    color: var(--fonte-color-1);
    align-items: center;
    border-radius: 12px;
    margin-left: 5%;
  }
  .conteudo_paragrafos {
    font-family: var(--fonte-secundaria);
    font-size: 1.375rem;
    margin-bottom: 2.5rem;
  }
  .conteudo_paragrafos h1 {
    font-family: var(--fonte-primaria);
    /* font-size: 40px; */
  }
  .conteudo_projetos {
    display: flex;
    justify-content: space-around;
    width: 100%;
    font-family: var(--fonte-primaria);
  }
  /* responsividade */
  @media (max-width: 56rem) {
    h1 {
      text-align: center;
    }
    .conteudo_projetos {
      flex-direction: column;
      align-items: center;
    }
  }
</style>
