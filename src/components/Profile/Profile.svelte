<script>
	import ProfilePicture from "./ProfilePicture.svelte";
	import ProfileQuote from "./ProfileQuote.svelte";
</script>

<div class="profile">
  <div class="profile-geral">
	  <ProfilePicture />
    <div class="profile-about">
      <h2 class="profile-about-title">Jhonatan Silva</h2>
      <h3 class="profile-about-subtitle">but can call me Jhowl</h3>
      <p class="profile-about-text">
          Back-end developer, passionate about technology and programming. I have been working with web development for 10 years,
          I have experience with PHP, NodeJS, ReactJS, React Native, VueJS, Laravel, CodeIgniter, MySQL, MongoDB, PostgreSQL, Docker, AWS, Digital Ocean, Linux, Git, among others.
      </p>
    </div>
  </div>
	<ProfileQuote />
</div>


<style>
	.profile {
		position: relative;
		top: 202px;
    width: 100%;
    height: 1000px;
    /* border: #FFFFFF 1px solid; */
	}

  .profile-geral {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 0 0 190px;
    /* border: #FFFFFF 1px solid; */

  }

  .profile-geral::after {
    display: inline-block;
  }

  .profile-about {
    flex-direction: column;
    justify-content: left;
    align-items: left;
    /* border: #FFFFFF 1px solid; */

  }

	.profile-about-title {
		width: 336px;
		height: 50px;
		left: 650px;
		top: 307px;

		font-weight: 600;
		font-size: 48px;
		line-height: 50px;

		color: #FFFFFF;
	}

	.profile-about-subtitle {
		/* position: absolute; */
		width: 450px;
		height: 38px;
		left: 650px;
		top: 368px;

		font-weight: 600;
		font-size: 36px;
		line-height: 38px;

		color: #FFFFFF;
	}

	.profile-about-text {
		/* position: absolute; */
		width: 324px;
		height: 85px;
		left: 650px;
		top: 456px;

		font-weight: 600;
		font-size: 24px;
		line-height: 25px;

		color: #FFFFFF;
	}

</style>
