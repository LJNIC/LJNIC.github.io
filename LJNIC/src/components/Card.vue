<template>
	<div class="card">
        <br>
		<p> {{ name }} </p>
        <br>
		<p> {{ description }} </p>
        <br>
	</div>
</template>

<script>
export default {
    props: {
        name: String,
        description: String
    },
    data () {
        return {
        }
    }
}
</script>

<style>
.card {
    text-align: center;
	color: lightgray;
	background: #21252b;
	border-radius: 5px;
    box-shadow: 4px 4px 4px black;
    font-size: 150%;
}
</style>
