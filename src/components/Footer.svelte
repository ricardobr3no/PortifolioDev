<script>
  import logo from "../assets/logo.png";
</script>

<footer>
  <p>Desenvolvido por Ricardo Aguiar</p>
  <div class="footer_logo">
    <img src={logo} alt="logo" />
  </div>
</footer>

<style>
  .footer_logo {
    scale: 0.6;
    position: relative;
    translate: 0px -2rem;
  }
  footer {
    height: 9rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: var(--background-color-2);
    color: white;
    font-family: var(--fonte-secundaria);
    font-size: 1.25rem;
    padding-top: 4rem;
    /* margin-top: 12rem; */
    /* margin-top: auto; */
  }
</style>
