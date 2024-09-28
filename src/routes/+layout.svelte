<header>
	<ul>
		<li>
			<h3>
				<a href="https://www.typescriptlang.org/docs/handbook/2/basic-types.html"
					>Documentation. BASIC</a
				>
			</h3>
		</li>
		<li>
			<h3>
				<a href="/simple">TS simple</a>
			</h3>
		</li>
		<li>
			<h3>
				<a href="https://www.typescriptlang.org/docs/handbook/2/basic-types.html"
					>Documentation. BASIC</a
				>
			</h3>
		</li>
		<li>
			<h3>
				<a href="https://www.typescriptlang.org/docs/handbook/2/basic-types.html"
					>Documentation. BASIC</a
				>
			</h3>
		</li>
	</ul>
</header>
<slot></slot>

<style>
	header {
		width: 1200px;
		margin: 0 auto;
	}
	:global(h1) {
		color: rgb(48, 48, 48);
	}
	ul {
		display: grid;
		grid-template-columns: repeat(4, minmax(70px, auto));
		align-items: center;
		justify-items: center;
		grid-auto-rows: auto;
		list-style: none;
		padding: 0rem 1rem;
		border: 1px solid #eee;
		border-radius: 0.5rem;
	}
	ul a {
		color: darkslategray;
	}
</style>
