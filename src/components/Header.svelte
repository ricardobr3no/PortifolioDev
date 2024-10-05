<script>
  import { Heart, Home, GraduationCap, SquareKanban } from "lucide-svelte";
</script>

<header>
  <nav class="navbar">
    <div class="navbar_buttons">
      <a href="/" class="navbar_buttons_item">
        <Home />
        <span>Home</span>
      </a>
      <a href="/habilidades" class="navbar_buttons_item">
        <GraduationCap />
        <span>Habilidades</span>
      </a>
      <a href="/projetos" class="navbar_buttons_item">
        <SquareKanban />
        <span>Projetos</span>
      </a>
    </div>
  </nav>
</header>

<style>
  .navbar {
    display: flex;
    align-items: center;
    justify-content: space-around;
    /* background-color: orange; */
  }
  .navbar_buttons {
    margin-top: 10px;
    /* background-color: orange; */
    display: flex;
    justify-content: space-around;
    width: 550px;
    height: 50px;
    background-color: var(--background-color-2);
    align-items: center;
    border-radius: 26px;
  }

  .navbar_buttons_item {
    color: #9b53b5;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 300px;
    height: 30px;
    /* background-color: white; */
    border-radius: 6px;
    text-decoration: none;
    font-family: var(--fonte-secundaria);
    font-size: 24px;
  }
  .navbar_buttons_item:hover {
    text-decoration: underline 2px;
  }
  .navbar_buttons_item span {
    margin-left: 10px;
  }
</style>
