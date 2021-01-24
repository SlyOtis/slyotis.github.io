<script lang="ts">
</script>

<style>
	img {
		user-select: none;
	}
	main {
		width: 100%;
		height: 100%;
		background-color: #e8d680;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		user-select: none;
	}
	.content {
		list-style: none;
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100%;
		max-width: 400px;
		height: auto;
		border: 1px solid black;
		border-radius: 8px;
		overflow: hidden;
		background-color: white;
		z-index: 1;
		position: relative;
		box-shadow: 0 5px 0 1px black;
		box-sizing: border-box;
		margin: 0;
		padding: 0;
	}
	.content li {
		width: 100%;
		height: auto;
		padding: 16px;
		box-sizing: border-box;
		cursor: pointer;
		z-index: 1;
		transition: box-shadow 200ms ease-in-out;
	}

	.content li:active .bck {
		transition: all 50ms ease-in;
		box-shadow: inset 0 0 5px 0 black;
	}

	.content li:active a{
		transition: all 50ms ease-in;
		opacity: 0.8;
	}

	.content li a {
		position: relative;
		z-index: 2;
		height: auto;
		user-select: none;
		transition: all 200ms ease-in;
		box-sizing: border-box;
		overflow: hidden;
	}

	.content li:hover .bck {
		transform: translateX(0);
		opacity: 1;
	}
	.content li:hover a {
		text-shadow: 0 0 5px #fff, 0 0 5px #fff;
		color: white;
	}
	.content li:not(:last-of-type) {
		border-bottom: 1px solid black;
	}
	.bck {
		position: absolute;
		top: 0;
		left: 0;
		bottom: 0;
		right: 0;
		transform: translateX(-100%);
		transform-origin: left center;
		transition: all 200ms ease-in;
		z-index: 1;
		opacity: 0;
		background: linear-gradient(
			to right,
			#78c5d6,
			#459ba8,
			#79c267,
			#c5d647,
			#f5d63d,
			#f08b33,
			#e868a2,
			#be61a5
		);
	}
</style>

<main>
	<img src="./slyotis.jpg" />
	<ul class="content">
		<li>
			<a>WaveForm Test</a>
			<div class="bck" />
		</li>
	</ul>
</main>
