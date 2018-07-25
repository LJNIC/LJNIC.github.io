<template>
	<div class="card">
        <a :href="url">
            <img :src="'/static/' + image"/>
        </a>
        <br>
        <slot name="description"></slot>
        <br>
	</div>
</template>

<script>
export default {
    props: {
        image: {
            type: String,
            required: true
        },
        url: {
            type: String,
            required: true
        } 
    },
    data () {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../variables.scss';
.card {
    text-align: center;
	color: $accent;
	background: $card-background;
	border-radius: 5px;
    box-shadow: 4px 4px 4px $shadow;
    font-size: $card-size; 
}

img {
	width: 100%;
	transition: all 0.3s;
	transform-origin: 50% 50%;
	max-width: 100%;
}

img:hover{
	transform: scale(1.05);
}
</style>
