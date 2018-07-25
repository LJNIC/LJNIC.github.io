<template>
  <div id="app">
    <div id="grid">
	  <TheTitleCard/>
    <GridCard 
      url="https://github.com/Atherys-Horizons"
      image="atherys.jpg"
      :description="`I'm part of the development team for an upcoming Minecraft RPG server. 
                     We use Java and an API called Sponge to develop plugins that interact 
                     with the game world.`"
    ></GridCard>
    <GridCard 
      url="https://github.com/LJNIC/Talro"
      image="menu.png"
    >
    <vue-markdown name="description"> A pyramid exploration roguelike game written with Lua and the LOVE game framework. It uses the fantastic [rotLove](https://github.com/paulofmandown/rotLove) library that I've modified with additional features.
    </vue-markdown>
    </GridCard>
    <GridCard 
      color="#f490e4"
      url="https://ljnic.github.io/rogueinlove"
      image="love.png"
      name="A Roguelike in LÖVE"
    >
    <vue-markdown name="description"> A tutorial for writing a roguelike with LOVE. The website is written in CSS     and HTML, save for the syntax highlighting, which is handled by [Hightlight.js](https://highlightjs.org/)
    </vue-markdown>
    </GridCard>
    </div>
    <GitHub/>
  </div>
</template>

<script>
import TheTitleCard from './components/TheTitleCard.vue'
import GridCard from './components/GridCard.vue'
import GitHub from './components/GitHub.vue'
import VueMarkdown from 'vue-markdown'

export default {
  name: 'app',
	components: {
		TheTitleCard,
    GridCard,
    GitHub,
    VueMarkdown
	},
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
@import 'variables.scss';
#grid {
  display: grid;
  grid-column-gap: 20px;
  grid-row-gap: 20px;
  justify-content: center;
  justify-self: center;
  grid-template-columns: 50% 50%;
}

body {
  margin-right: 4%;
  margin-left: 4%;
  margin-top: 0;
  padding: 4%;
  margin-bottom: 0;
  background: $background;
  font-family: 'Oxygen', sans-serif;
}

p {
  margin-bottom: 0;
  margin-top: 0;
}

@media screen and (max-width: 600px) {
  #app {
    grid-template-columns: 100%;
  }
}

</style>
