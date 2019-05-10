<template>
    <div>
		<v-carousel>
			<v-carousel-item v-for="m in imagens" :key="m.link" :src="m.link">
			</v-carousel-item>
		</v-carousel>		
	</div>
</template>
<script>
export default {
	data(){
		return{
			imagens:[
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"},
				{link: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg"}
			]
		}
	}
}
</script>

