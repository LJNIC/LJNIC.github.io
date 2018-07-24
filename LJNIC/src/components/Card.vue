<template>
	<div class="card">
        <a :href="url">
            <img :src="'/static/' + image"/>
        </a>
        <br>
		<p> {{ description }} </p>
        <br>
	</div>
</template>

<script>
export default {
    props: {
        name: String,
        description: String,
        image: String,
        color: String,
        url: String
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
    font-size: 115%;
}

img {
    max-width: 100%;
}
</style>
