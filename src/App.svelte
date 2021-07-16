
<script >
  	import {Rive} from 'rive-js'
	import {onMount} from 'svelte'
	
	let canvas,rive
	onMount(() => {
		rive = new Rive({
		   src: 'rive_test.riv',
		  canvas:canvas,
		  autoplay: true,
	  });
	})
</script>
<main>
<canvas bind:this={canvas} width={1280} height={722}></canvas>
</main>

<style>
	main{
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>