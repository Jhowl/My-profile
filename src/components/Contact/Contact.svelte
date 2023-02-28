<script>

</script>

<div class="contact">

  <form action="https://formspree.io/f/xaylqzqo" method="POST">
    <input type="text" name="name" placeholder="Your name">
    <input type="email" name="_replyto" placeholder="Your email">
    <textarea name="message" placeholder="Your message"></textarea>
    <button type="submit">Send</button>
  </form>
</div>

<style>
  .contact {
    position: relative;
    width: 100%;
    margin-bottom: 50px;
  }

  form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  input, textarea {
    width: 100%;
    margin-top: 20px;
    color: white;
    background: rgba(217, 217, 217, 0.4);
    border-radius: 12px;
  }

  input {
    width: 745px;
    height: 39px;
  }

  textarea {
    width: 745px;
    height: 233px;
    padding-top: 10px;
    margin-bottom: 30px;
  }

  input::placeholder, textarea::placeholder{
    color: #ffffff;
    font-family: 'Inconsolata', monospace;
    /* padding-top: 10px; */
    padding-left: 5px;
  }

</style>
