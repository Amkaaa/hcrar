<template>
    <div class="notFound">
      <div>
        <h1>Уучлаарай таны хайж байгаа хуудас байхгүй байна.</h1>
        <img src="../assets/img/404.svg" alt="">
      </div>
    </div>
</template>

<script>
export default {
  name: 'NotFound',
  components: {

  }
}
</script>
<style lang="css" scoped>
  .notFound{
    margin: 0;
    padding: 0;
    min-height: calc(100vh - 115px);
    font-family: 'Roboto Condensed', sans-serif;
  }
  .notFound div{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  h1 {
    margin: 0;
    font-weight: 100;
    font-size: 2em;
  }
  img {
    width: 40em;
  }
</style>