<template>
  <div id="app">
	  <TitleCard/>
    <Card 
      name="A'therys Horizons" 
      description="I'm part of the development team for an upcoming Minecraft RPG server. We use Java and an API called Sponge."
    ></Card>
    <Card 
      name="Talro"
      description="A pyramid exploration roguelike game written with Lua and the LOVE game framework."
    ></Card>
    <Card 
      name="A Roguelike in LOVE"
      description="A tutorial for writing a roguelike with LOVE. Hand written CSS and HTML, save for syntax highlighting."
    ></Card>
  </div>
</template>

<script>
import TitleCard from './components/TitleCard.vue'
import Card from './components/Card.vue'

export default {
  name: 'app',
	components: {
		TitleCard,
    Card
	},
  data () {
    return {
    }
  }
}
</script>
<style>
  #app {
    display: grid;
    grid-column-gap: 20px;
    grid-row-gap: 20px;
    justify-content: center;
    justify-self: center;
    grid-template-columns: 50% 50%;
  }

  @media screen and (max-width: 600px) {
	  #app {
      grid-template-columns: 100%;
    }
}
</style>
