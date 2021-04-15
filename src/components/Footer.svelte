<footer
  class="site-footer bg-image overlay "
  style="background-image: url('images/hero-bg.jpg'); background-attachment:fixed; "
>
  <div class="container">
    <div class="row">
      <div class="col-12 text-center mb-5">
        <h3 class="text-white">Molten Massage</h3>
      </div>
      <div class="col-12 text-center mb-5">
        <!-- svelte-ignore a11y-invalid-attribute -->
        <a href="/" class="">Home</a>
        <span class="mx-3" />
        <a href="/about" class="">About</a>
        <span class="mx-3" />
        <a href="/service" class="">Services</a>
        <span class="mx-3" />
        <a href="/contact" class="">Contact</a>
      </div>
      <div class="col-12">
        <div class="social white text-center">
          <a href="#"><span class="icon-twitter" /></a>
          <a href="https://www.instagram.com/buckleballa41"
            ><span class="icon-instagram" /></a
          >
          <a href="#"><span class="icon-facebook" /></a>
          <a href="#"><span class="icon-linkedin" /></a>
        </div>
      </div>
    </div>
    <div class="row pt-5 mt-5 text-center">
      <div class="col-md-12">
        <div class="border-top pt-5">
          <p class="small text-white">
            Copyright ©
            <script>
              document.write(new Date().getFullYear());
            </script>2021
            <br />
            Molten Massage All rights Reserved
          </p>
        </div>
      </div>
    </div>
  </div>
</footer>

<style>
  footer .container {
    padding: 4rem 0;
  }
  .social.white a {
    background: #fff3;
  }

  .social span {
    margin-top: 13px;
    line-height: 50px;
  }
  .social a {
    display: inline-block;
    font-size: 1.5rem;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    background: #ffa18833;
    position: relative;
  }
  .site-footer a {
    color: #ffffffec;
    font-family: "Open Sans", sans-serif;
  }
  .site-footer a:hover {
    color: #ffa288;
    text-decoration: none;
  }
  .site-footer .border-top {
    border-top: 1px solid #ffffff1a !important;
  }
</style>
