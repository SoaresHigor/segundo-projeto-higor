<template>
  <header>
  <div class="hello">
    <h1>Conheça Aripuanã!</h1>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Fv_raZQM72s?si=sMVT0n4c5Syi4MTi" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    
    <nav>
    <ul>
      <li><a href="#fotos">Fotos</a></li>
      <li><a href="#rotas">Pontos Turísticos</a></li>
      <li><a href="#destinos">Destinos</a></li>
    </ul>
  </nav>
      </div>
    </header>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
  color: rgb(38, 75, 3);
}
h2 {
  color: #000000;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-flex;
  margin: 0 10px;
  color: #000000;
}
a {
  color: #000000;
}
</style>
