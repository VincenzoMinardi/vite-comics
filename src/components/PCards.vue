<script>

export default {
    props: {
       urlImg: String,
	   title: String,
	   price: String,

    },
};

</script>
<template>
	<div class="card">
		<div class="container-image">
			<img :src="urlImg" :alt="title">
		</div>
		<div class="text-container">
			<p>{{title}}</p>
			<p>{{price}}</p>
		</div>
		
	</div>
	
	
</template>

<style lang="scss">
.card{
width: calc((100% / 6) - 1rem);
margin: 1.5rem 0.5rem;

.container-image{
	width: 100%;
	height: 100%;
	aspect-ratio: 1 / 1;

	
	img{
		width: 100%;
		height: 100%;
		object-fit: cover;
	}
}

.text-container{
	color: white;
	font-size: 0.9em;
	text-align: center;
	margin-top: 1.3rem;

}


}

</style>





