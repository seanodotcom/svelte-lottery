<script>
	import '../app.postcss';
</script>

<div class="navbar">
	<a href="/">Home</a>
	<a href="/results">Results</a>
</div>

<div class="container">
	<slot />
</div>

<style>
    .navbar {
        display: flex;
        justify-content: space-between;
        background-color: #333;
        color: #eee;
        padding: 10px;
		margin-bottom: 1em;
    }
    .navbar a {
        color: #eee;
        text-decoration: none;
        padding: 4px;
    }
    .navbar a:hover {
        color: #ccc;
    }
    .navbar a.active {
        border: 1px solid #ccc;
        border-radius: 4px;
    }

    :global(body) {
        margin: 0;
    }
    .container {
        max-width: 90%;
        margin: 0 auto;
        width: 1200px;
    }
</style>
