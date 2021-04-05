<template>
  <div class="header container">
    <h6 class="small text-white">Cotizador</h6>
    <h6 class="subtitle text-dark">Citadino, Aventurero, Deportivo</h6>
    <h1 class="title text-white display-1">Elige el tuyo</h1>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
    margin-top: 2.25rem;
}

h6 {
    &.small {
        text-transform: uppercase;
        font-size: 0.6rem;
        letter-spacing: 0.3rem;
        font-weight: 700;
    }
}

h6 {
    &.subtitle {
        margin-top: 1.25rem;
        font-family: 'Playfair Display', sans-serif;
        text-transform: uppercase;
        justify-content: center;
        display: flex;
        width: 100%;
        align-items: center;
        font-size: 0.9rem;
        letter-spacing: 0.6px;
        font-weight: 700;

        &::before,&::after {
            content: '';
            background-color: rgb(0, 0, 0);
            height: 0.1rem;
            margin: .5rem;
            width: 3.5rem;
        }
    }
}

h1 {
    &.title {
        font-family: 'Playfair Display', sans-serif;
        font-weight: 900;
        font-style: italic;
    }
}
</style>
