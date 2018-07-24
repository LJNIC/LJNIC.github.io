<template>
  <div id="app">
	  <TitleCard/>
    <Card 
      color="#ff9400"
      url="https://github.com/Atherys-Horizons"
      image="atherys.jpg"
      name="A'therys Horizons" 
      description="I'm part of the development team for an upcoming Minecraft RPG server. We use Java and an API called Sponge."
    ></Card>
    <Card 
      color="#dca456"
      url="https://github.com/LJNIC/Talro"
      image="menu.png"
      name="Talro"
      description="A pyramid exploration roguelike game written with Lua and the LOVE game framework."
    ></Card>
    <Card 
      color="#f490e4"
      url="https://ljnic.github.io/rogueinlove"
      image="love.png"
      name="A Roguelike in LÖVE"
      description="A tutorial for writing a roguelike with LÖVE. Hand written CSS and HTML, save for syntax highlighting."
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
