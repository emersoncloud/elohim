<script lang="ts">
	import Header from './Header.svelte';
	import SaveState from "./SaveState.svelte";
	import Players from './Players.svelte';
	import CreatePlayer from "./CreatePlayer.svelte";
	import Teams from './Teams.svelte'
	import HowTo from "./HowTo.svelte";
</script>

<main>
	<Header/>
	<div class='motherload'>
		<div class='daughterload'>
			<SaveState />
			<HowTo />
			<CreatePlayer />
			<Players />
			<Teams />
		</div>
	</div>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		text-align: center;
		font-family: Georgia, 'Times New Roman', Times, serif;
		width: 100%;
		background: linear-gradient(black 10%, #212121 50%, black 100%);
	}

	.motherload {
		display: flex;
		padding: 20px;
		justify-content: center;
	}

	.daughterload {
		max-width: 1100px;
		width: 100%;
	}


	:global(body) {
		padding: 0;
		background-color: black;
		transition: background-color 0.3s;
	}
</style>