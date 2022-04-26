<script>
	import {continents, indicateurs} from '$lib/listing.js';
</script>


<section>
	<p> Continent </p>
	<ul>
	{#each continents as cont}
		<div class="cont">{cont.nameC}</div>
		{#each cont.countries as country}
			<div class="card">{country.nameP}</div>
		{/each}
	{/each}
	</ul>

	
	
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	p {
		color:pink;

	}
	.cont{
		color:blue;

	}
	.card {
		border:solid 1px red;
		width: 120%;
		margin: 10px;
		padding: 10px; 
		color: green; 
	}
	
</style>
