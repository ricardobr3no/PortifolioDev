<script>
  import { Linkedin, Github, Mail } from "lucide-svelte";
</script>

<div class="conteudo_redes">
  <h3>Minhas Redes</h3>
  <div class="conteudo_redes_container">
    <a href="/" class="conteudo_redes_item">
      <Github />
      <span>Github </span>
    </a>
    <a href="/" class="conteudo_redes_item">
      <Linkedin />
      <span>Linkedin </span>
    </a>
    <a href="/" class="conteudo_redes_item">
      <Mail />
      <span>Email</span>
    </a>
  </div>
</div>

<style>
  .conteudo_redes {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
  }
  .conteudo_redes h3 {
    font-family: var(--fonte-primaria);
  }
  .conteudo_redes_container {
    display: flex;
    justify-content: space-around;
    align-items: center;
    /* background-color: red; */
    width: 100%;
  }
  .conteudo_redes_item {
    display: flex;
    align-items: center;
    justify-content: center;

    width: 130px;
    height: 45px;
    background-color: var(background-color-1);
    color: var(--fonte-color-2);
    border-radius: 6px;
    text-decoration: none;
    flex-wrap: wrap;
    border: solid 2px var(--fonte-color-2);
    font-family: var(--fonte-primaria);
  }
  .conteudo_redes_item span {
    margin-left: 10px;
    color: white;
  }

  .conteudo_redes_item:hover {
    background-color: var(--background-color-2);
  }
</style>
