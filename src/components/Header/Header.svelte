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
	<div class="header-wrapper">
    <h1 class="header-title">{title}</h1>
    <div class="nav-wrapper">
      <nav class="header-nav">
        <ul>
          {#each navOptions as option}
          <li class="header-nav-item">
            <a href={option.href}>{option.label}</a>
          </li>
          {/each}
          <li class="header-nav-item toggle">
            <input type="checkbox" id="toggle" on:change={toggleTheme}>
            <label for="toggle">
              <img src="icons/icon-light-bulb.svg" alt="Light Mode" class="light-mode">
            </label>
          </li>
        </ul>
      </nav>
    </div>
  </div>

  <div class="github-header">
    <a href="{link}" target="_blank" rel="noopener noreferrer">
      <img src="icons/github-icon.svg" alt="Github">
    </a>
	</div>

</header>
<style>
	.header {
		width: 100%;
		height: 116px;
		left: 0px;
		top: 0px;
    position: relative;
		background: #000002;
	}

  .header-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 4rem;
  }

	.header-title {
		position: relative;
		width: 144px;
		height: 50px;
		left: 104px;
		top: 0px;
	}

	.header-nav {
		width: 672px;
		height: 25px;
		left: 395px;
		top: 14px;

		font-weight: 700;
		font-size: 24px;
		line-height: 25px;

    display: flex;
    width: 100%;
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
    width: 100%;
	}

	.header-nav-item {
		margin-right: 20px;
	}

	 .toggle {
		width: 28.38px;
		height: 37.3px;
		left: 1138px;
		top: 37.95px;
	}

	.toggle input[type="checkbox"] {
		display: none;
	}

	.github-header {
		position: absolute;
		width: 65px;
		height: 457px;
    top: 380px;
    right: 5%;
	}

  .github-header::before {
    content: "";
    background: white;
    width: 1px;
		height: 380px;
    position: absolute;
    top:  -420px;
    left: 50%;
  }

  .navbar {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1;
  }

  .navbar--scrolled {
		width: 100%;
		height: 116px;
		left: 0px;
		top: 0px;

    z-index: 10;
  }

  .nav-wrapper {
    display: flex;
    align-items: center;
    width: 80%;
    padding: 0 10%;
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
