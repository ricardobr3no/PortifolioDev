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
    translate: 0px -30px;
  }
  footer {
    height: 150px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: var(--background-color-2);
    color: white;
    font-family: var(--fonte-secundaria);
    font-size: 20px;
    padding-top: 70px;
    margin-top: 200px;
  }
</style>
