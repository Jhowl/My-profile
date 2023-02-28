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
          <!-- I have experience with PHP, NodeJS, ReactJS, React Native, VueJS, Laravel, CodeIgniter, MySQL, MongoDB, PostgreSQL, Docker, AWS, Digital Ocean, Linux, Git, among others. -->
      </p>
    </div>
  </div>
	<ProfileQuote />
</div>

<style>
	.profile {
		position: relative;
		top: 109px;
    width: 100%;
    height: 800px;
    display: flex;
    flex-direction: column;
    /* add margem down */
    margin-bottom: 150px;
	}

  .profile-geral {
    position: relative;
    display: flex;
    height: 100%;
    align-items: center;
  }

  .profile-about {
    display: inline;
    width: 100%;
  }

	.profile-about-title {
		font-weight: 600;
		font-size: 48px;
		line-height: 50px;
    margin-top: 0;
		color: #FFFFFF;
	}

	.profile-about-subtitle {
		font-weight: 600;
		font-size: 36px;
		line-height: 38px;

		color: #FFFFFF;
	}

	.profile-about-text {
		width: 34%;
		font-weight: 600;
		font-size: 24px;
		line-height: 25px;

		color: #FFFFFF;
	}

</style>
