<script>
  export let title = "nome do projeto";
  // let description = "Esta é uma descrição curta sobre o cartão.";
  export let imageUrl = "https://placehold.co/300x200";
  export let source = "/";
</script>

<a class="card" href={source}>
  <img src={imageUrl} alt="Imagem do cartão" />
  <h3>{title}</h3>
  <!-- <p>{description}</p> -->
</a>

<style>
  .card {
    text-decoration: none;
    display: flex;
    flex-direction: column;
    width: 18rem;
    height: 18rem;
    /* border: 1px solid #ccc; */
    padding: 0.625rem;
    justify-content: center;
    align-items: center;
    color: var(--fonte-color-2);
    /* border-radius: 5px; */
    /* box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); */
  }
  .card img {
    border-radius: 20px;
    /* object-fit: scale-down; */
    height: 12.5rem;
    width: 18rem;
  }

  .card:hover {
    text-decoration: underline 2px;
    scale: 1.07;
  }
</style>
