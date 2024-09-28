<script>
	import { readable } from 'svelte/store'
	const object = { message: 'Hello TS!' }
	const date = readable(new Date(), (set) => {
		set(new Date())
		const interval = setInterval(() => {
			set(new Date())
		}, 1000)
		return () => clearInterval(interval)
	})
	$: time = $date
</script>

<h2>Type Script Simple</h2>
<h3>{object.message}</h3>
<ul>
	<li>{`${time.getHours()} : ${time.getMinutes()} : ${time.getSeconds()}`}</li>
	<li>{time.toDateString()}</li>
</ul>

<style>
	h3 {
		width: 1200px;
		margin: 1rem auto;
		text-align: start;
		color: darkslategrey;
	}
	ul {
		position: absolute;
		top: 0;
		right: 2rem;
		/* margin: 0;
		padding: 0; */
		list-style: none;
	}
</style>
