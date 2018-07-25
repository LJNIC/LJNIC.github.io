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

<style>
 #title-card {
	font-size: 500%;
	border-bottom: solid lightgray;
	border-right: solid lightgray;
	padding-right: 4%;
	padding-bottom: 2%;
	text-align: right;
	color: #217c59;
	background: #15181c;
	font-family: 'Inconsolata', monospace;
  width: 100%;
  box-sizing: border-box;
  display: table;
} 

.center {
  display: table-cell;
  vertical-align: middle;
  width: 100%;
  height: 100%;
}
</style>
