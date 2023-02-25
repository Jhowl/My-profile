<script>
	import Header from './components/Header/Header.svelte';
	import Profile from './components/Profile/Profile.svelte';
	import Skills from './components/Skills/Skills.svelte';
  import Projects from './components/Projects/Projects.svelte';
  import Contact from './components/Contact/Contact.svelte';
</script>

<Header />
<Profile />
<Skills />
<Projects />
<Contact />

<footer>
  <div class="footer">
    <p>© Jhowl - 2023.</p>
  </div>
</footer>

<style>
  footer {
    position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
    text-align: center;
    background-color: #333333;
    color: #ffffff;
    padding: 10px 0;
  }

  .footer p {
    margin: 0;
  }

</style>
