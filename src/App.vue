<template>
  <div id="app">
    <Header/>
    <div class="board">
      <div class="lane"><h2 class="lane-title">Backlog</h2></div>
      <div class="lane"><h2 class="lane-title">Desenvolvimento</h2></div>
      <div class="lane"><h2 class="lane-title">Testes</h2></div>
      <div class="lane"><h2 class="lane-title">Concluídos</h2></div>
    </div>
  </div>
</template>

<script>
import Header from './components/Header';
export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style>
.board{
  display: flex;
  justify-content: flex-start;
  margin: 1.2rem 0.8rem;
}

.lane{
  background: var(--color-grey);
  width: 23rem;
  height: 30rem;
  border-radius: 0.8rem;
  box-shadow: 0 .1rem .2rem 0 rgba(33,33,33,0.1);
  margin: 0 0.8rem;
}
</style>
