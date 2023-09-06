<div id="navbar">
	<p>📦 EarlySoftware</p>
</div>

<style>
	:root {
		--navbar-height: 50px;
	}

	#navbar {
		width: 100%;
		height: var(--navbar-height);

		border-bottom: black solid 2px;
		font-family: 'Rubik';

		background-color: var(--background-color);
		position: relative;
		z-index: 500;
	}

	img {
		width: 30px;
		vertical-align: middle;
	}

	#navbar p {
		color: black;
		font-weight: 700;
		font-size: 1.4em;

		line-height: var(--navbar-height);

		text-overflow: ellipsis;
		white-space: nowrap;
	}
</style>
