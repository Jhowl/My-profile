<script>

</script>

<div class="skills">
	<div class="skills-header">
		<div class="skill-rectangle1"></div>
		<div class="skill-rectangle2"></div>
		<h2 class="skill-title">skills.</h2>
	</div>

  <div class="skills-container">
      <div class="skill-item">
        <h2>Basic</h2>
        <button class="btn-white">C#</button>
        <button class="btn-white">C++</button>
        <button class="btn-white">Java</button>
      </div>

      <div class="skill-item">
        <h2>Intermediate</h2>
        <button class="btn-orange-dark">Python</button>
        <button class="btn-orange-dark">React</button>
        <button class="btn-orange-dark">Svelte</button>
        <button class="btn-orange-dark">HTML</button>
        <button class="btn-orange-dark">CSS</button>
        <button class="btn-orange-dark">Go</button>
        <button class="btn-orange-dark">Docker</button>
      </div>

      <div class="skill-item">
        <h2>Advanced</h2>
        <button class="btn-orange-glow">NodeJs</button>
        <button class="btn-orange-glow">Javascript</button>
        <button class="btn-orange-glow">PHP</button>
        <button class="btn-orange-glow">Wordpress</button>
        <button class="btn-orange-glow">Rest API</button>
        <button class="btn-orange-glow">Woocommerce</button>
        <button class="btn-orange-glow">MongoDB</button>
        <button class="btn-orange-glow">MySQL</button>
      </div>
    </div>
  </div>

<style>
	.skills {
		position: relative;
    width: 100%;
    height: 400px;
	}

  .skills-header::after {
    content: '';
    position: absolute;
    width: 90%;
    height: 1px;
    bottom: 2px;
    background: white;
    right: 0;
    z-index: -1;
    margin-right: 160px;
  }

	.skills-header {
		position: relative;
		font-weight: 700;
		font-size: 48px;
    width: 100%;
		color: #B65D00;
	}

  .skill-title {
    position: relative;
    left: 144px;
    /* top: 947px;  */
  }

	.skill-rectangle1 {
		box-sizing: border-box;
		position: absolute;

    width: 137px;
    height: 69px;
    left: 12px;
    bottom: 50px;

		background: #000002;
		border: 2px solid #DEDEDE;
		border-radius: 25px;
    z-index: 1;
	}

	.skill-rectangle2 {
		box-sizing: border-box;
    width: 105px;
    height: 105px;
		position: absolute;

		left: -28px;
    bottom: 10px;

		background: #000002;
		border: 2px solid #DEDEDE;
		border-radius: 25px;
	}

  .skills-container {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 30px 0 30px;
    margin-right: 140px;
    margin-left: 140px;

  }

	.skill-item {
    position: relative;
    width: 60%;
    height: 100%;
	}


	.btn-white{
		background: #D9D9D9;
		border-radius: 10px;

		border-radius: 10px;
		padding: 5px 10px 5px 10px;
		margin-top: 10px;
		font-weight: 700;
		font-size: 16px;
	}

	.btn-orange-glow{
		background: #FB8D27;
		border-radius: 10px;
		padding: 5px 10px 5px 10px;
		margin-top: 10px;
		font-weight: 700;
		font-size: 16px;
	}

	.btn-orange-dark{
		background: #B65D00;
		border-radius: 10px;

		border-radius: 10px;
		padding: 5px 10px 5px 10px;
		margin-top: 10px;
		font-weight: 700;
		font-size: 16px;
	}

</style>
