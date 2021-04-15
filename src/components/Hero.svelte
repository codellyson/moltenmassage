<script>
  export let pageHeading;
  export let pageIntro;
</script>

<div class="ftco-blocks-cover-1">
  <div
    class="site-section-cover overlay"
    data-stellar-background-ratio="0.5"
    style="background-image: url(images/hero-bg.jpg); background-position: center; background-repeat:no-repeat; background-size:cover; background-attachment:fixed;"
  >
    <div class="container">
      <div class="row align-items-center">
        <div class="col-md-7">
          <h1 class="mb-3">{pageHeading}</h1>
          <p class="py-3">{pageIntro}</p>
          <p><a href="/about" class="btn btn-primary">Learn More</a></p>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  .site-section-cover {
    background-position: 50% 50%;
  }
  .site-section-cover h1 {
    font-size: 4rem;
    color: #fff;
    line-height: 1.5;
    font-family: "Playfair Display", serif;
    font-weight: 900;
  }
  .site-section-cover p {
    font-size: 20px;
    color: #fff;
    font-family: "Open Sans", serif;
    margin: 2rem 0;
  }
  .site-section-cover.overlay {
    position: relative;
  }
  .site-section-cover,
  .site-section-cover .container {
    position: relative;
    z-index: 2;
  }
  /* .site-section-cover,
  .site-section-cover .container > .row {
    height: calc(100vh - 196px);
    min-height: 677px;
  } */
  .site-section-cover,
  .site-section-cover .container > .row {
    min-height: 100vh;
  }
  .site-section-cover.overlay:before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: #00000071;
    z-index: 1;
  }
  @media (min-width: 768px) {
    .site-section-cover h1 {
      font-size: 3rem;
    }
  }
</style>
