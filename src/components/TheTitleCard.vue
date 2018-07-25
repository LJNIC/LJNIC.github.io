<template>
	<div id="title-card">
    <span class="center">
		<p> Liam's </p>
		<p> Projects </p>
    </span>
	</div>
</template>

<script>
export default {
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../variables.scss';
#title-card {
	font-size: $title-size;
	border-bottom: solid $accent;
	border-right: solid $accent;
	padding-right: 4%;
	padding-bottom: 2%;
	text-align: right;
	color: $title;
	background: $background;
	font-family: 'Inconsolata', monospace;
  width: 100%;
	height: 100%;
  box-sizing: border-box;
  display: table;
} 

#github {
	max-width: 200px;
	float: left;
}

.center {
  display: table-cell;
  vertical-align: middle;
  width: 100%;
  height: 100%;
}
</style>
