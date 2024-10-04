<script>
  import Header from "../../components/Header.svelte";
  import Footer from "../../components/Footer.svelte";
  import Card from "../../components/Card.svelte";
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
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut aliquam
          sed quas blanditiis laboriosam corporis, accusantium, nihil nostrum
          sunt quo ipsam voluptate. Nihil asperiores et dicta eius similique
          voluptas dolores.
        </p>
      </div>
      <div class="conteudo_projetos">
        <Card />
        <Card />
        <Card />
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
    height: 100vh;
    margin-left: 150px;
    margin-right: 150px;
    /* justify-content: space-around; */
  }
  .conteudo {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    /* margin: 50px; */
    color: var(--fonte-color-1);
    align-items: center;
    border-radius: 12px;
  }
  .conteudo_paragrafos {
    font-family: var(--fonte-secundaria);
    font-size: 22px;
    margin-bottom: 40px;
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
</style>
