<script>
	export let title = "jhowl.";
	export let navOptions = [
		{ label: "Profile.", href: "#profile" },
		{ label: "Skills.", href: "#skills" },
		{ label: "Projects.", href: "#projects" },
		{ label: "Contact.", href: "#contact" },
	];

	let isDarkMode = false;

	export let link = "https://github.com/your-github-username";

	function toggleTheme() {
		isDarkMode = !isDarkMode;
		document.body.classList.toggle("light-mode", isDarkMode);
	}

	let scrollPosition = 0;

  window.addEventListener('scroll', () => {
    scrollPosition = window.pageYOffset;
  });
</script>

<header class="header {scrollPosition > 0 ? 'navbar navbar--scrolled' : 'navbar'}">
	<h1 class="header-title">{title}</h1>
	<nav class="header-nav">
		<ul>
			{#each navOptions as option}
			<li class="header-nav-item">
				<a href={option.href}>{option.label}</a>
			</li>
			{/each}
		</ul>
	</nav>

	<div class="toggle">
		<input type="checkbox" id="toggle" on:change={toggleTheme}>
		<label for="toggle">
			<img src="icons/light-bulb-icon.svg" alt="Light Mode" class="light-mode">
		</label>
	</div>

	<a href="{link}" target="_blank" rel="noopener noreferrer" class="github-header">
		<img src="icons/github-icon.svg" alt="Github">
	</a>
	<div class="line"></div>
</header>

<style>
	.header {
		position: absolute;
		width: 100%;
		height: 116px;
		left: 0px;
		top: 0px;

		background: #000002;
	}

	.header-title {
		position: absolute;
		width: 144px;
		height: 50px;
		left: 104px;
		top: 0px;
	}

	.header-nav {
		position: absolute;
		width: 672px;
		height: 25px;
		left: 395px;
		top: 14px;

		font-weight: 700;
		font-size: 24px;
		line-height: 25px;
	}

	 .header-nav a {
		color: #FFFFFF;

		text-decoration: none;
		font-weight: bold;
		font-size: 1.1rem;
	}

	.header-nav ul {
		list-style: none;
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
	}

	.header-nav-item {
		margin-right: 20px;
	}

	 .toggle {
		position: absolute;
		width: 28.38px;
		height: 37.3px;
		left: 1138px;
		top: 37.95px;

		/* background: #D9D9D9; */
	}

	.toggle input[type="checkbox"] {
		display: none;
	}

	.github-header {
		position: absolute;
		width: 65px;
		height: 457px;
		left: 86.23%;
		top: 200px;
	}

	.line {
		position: absolute;
		width: 380px;
		height: 0px;
		left: 77%;
		top: 0px;

		border: 1px solid #FFFFFF;
		transform: rotate(90deg);
	}

  .navbar {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1;
    /* other styles... */
  }

  .navbar--scrolled {
		width: 100%;
		height: 116px;
		left: 0px;
		top: 0px;

    z-index: 10;

  }

	/* .toggle span:before {
		content: "🌙";
	}

	.toggle span:after {
		content: "☀️";
	}

	.toggle input[type="checkbox"]:checked + span:before {
		display: none;
	}

	.toggle input[type="checkbox"]:checked + span:after {
		display: inline;
	} */

	/* .light-mode {
		background-color: #1a202c;
		color: #f5f5f5;
	}

	.light-mode .header__nav a {
		color: #f5f5f5;
	}  */
</style>
