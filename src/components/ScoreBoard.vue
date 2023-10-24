<template>
  <section class="score">
    Jogador <span>{{ this.win_count }}</span> x 
   <span>{{ this.lose_count }}</span> Computador
  </section>
</template>

<script>
 export default {
    props: {
        win_count: {
            type: Number,
            default: 0
        },
        lose_count: {
            type: Number,
            default: 0
        }
    }
 }
</script>

<style lang="scss" scoped>
section.score {
  border-bottom: 1px solid black;
  padding: 24px;
  font-size: 18px;

  span {
    padding: 8px;
    font-weight: bold;
    border: 1px solid black;
  }
}
</style>