<script>
  const teams = [
    {
      image: "images/founder.jpg",
      name: "John Smith",
      post: "Founder",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork ",
      id: 1,
    },
    {
      image: "images/founder.jpg",
      name: "John Smith",
      post: "Founder",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork ",
      id: 2,
    },
    {
      image: "images/founder.jpg",
      name: "John Smith",
      post: "Founder",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork ",
      id: 3,
    },
    {
      image: "images/founder.jpg",
      name: "John Smith",
      post: "Founder",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork ",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "John Smith",
      post: "Founder",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork ",
      id: 5,
    },
    {
      image: "images/founder.jpg",
      name: "John Smith",
      post: "Founder",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork ",
      id: 6,
    },
  ];
  import Promo from "../components/CTA.svelte";
  import Hero from "../components/Hero.svelte";
</script>

<style>
  .site-section {
    padding: 7rem 0;
  }
  .social-icons a {
    display: inline-block;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: #ffa18833;
    position: relative;
    font-size: 1.5rem;
    text-align: center;
  }
  .social-icons a:hover {
    color: #ffa288;
    text-decoration: none;
  }
  .social-icons span {
    margin-top: 13px;
    line-height: 50px;
  }
  .icon-twitter:before {
    content: "\f099";
  }
  .post-entry-1.person-1 .post-entry-1-contents {
    padding-top: 4rem;
  }
  .post-entry-1 .post-entry-1-contents {
    background: #fff;
    padding: 20px;
  }
  .post-entry-1.person-1 {
    text-align: center;
  }
  .post-entry-1.person-1 img {
    width: 90px;
    border-radius: 50%;
    margin: 0 auto -45px auto;
    border: 10px solid #fff;
  }
  .post-entry-1 .meta {
    color: #ccc;
  }
  .post-entry-1 .post-entry-1-contents h2 {
    font-size: 22px;
    margin-bottom: 20px;
  }
  p {
    margin-top: 0;
    margin-bottom: 1rem;
  }
</style>

<Hero pageHeading="About Us" />
<section id="about">
  <div class="site-section py-5 my-5">
    <h1 class="section-header-text text-center py-3">About Us</h1>
    <div class="container">
      <div class="row align-items-center">
        <div class="col-md-5 mr-auto mb-5">
          <h2 class="serif font-weight-bold mb-3">
            WellSpa Spa &amp; Wellness
          </h2>
          <p class="font-weight-bold">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum,
            consequuntur?
          </p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ea
            nesciunt, amet officia soluta, dolores dolor?
          </p>
          <div class="social-icons py-4">
            <a href="#"><span class="icon-twitter" /></a>
            <a href="#"><span class="icon-instagram" /></a>
            <a href="#"><span class="icon-facebook" /></a>
            <a href="#"><span class="icon-linkedin" /></a>
          </div>
        </div>
        <div class="col-md-6">
          <div class="d-flex align-items-center">
            <div
              class="bg-img-1 mr-md-4 mt-md-5"
              style="background-image:url(../images/green-plant.jpg" />
            <div
              class="bg-img-1"
              style="background-image:url(../images/green-plant.jpg)" />
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Side Two -->
  <div class="site-section bg-light">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2 class="section-header-text text-black mb-5 text-center">
            Our Team
          </h2>
        </div>
      </div>
      <div class="row align-items-stretch">
        {#each teams as team}
          <div class="col-lg-4 col-md-6 mb-5">
            <div
              class="post-entry-1 h-100 person-1 aos-init aos-animate"
              data-aos="fade-up"
              data-aos-delay="{team.id}00">
              <!-- svelte-ignore a11y-img-redundant-alt -->
              <img src={team.image} alt="Image" class="img-fluid" />
              <div class="post-entry-1-contents ">
                <span class="meta">{team.post}</span>
                <h2>{team.name}</h2>
                <p>{team.desc}</p>
              </div>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
  <!-- Three -->
  <div class="site-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 mb-5 mb-lg-0">
          <div
            class="img-years aos-init aos-animate"
            data-aos="fade-left"
            data-aos-delay="400">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src="images/green-plant.jpg" alt="Image" class="img-fluid" />
          </div>
        </div>
        <div
          class="col-lg-5 ml-auto pl-lg-5 text-center aos-init aos-animate"
          data-aos="fade-right"
          data-aos-delay="400">
          <h2
            class="heading-border-bottom font-weight-bold serif text-black mb-5 text-center">
            Why Us
          </h2>
          <p class="mb-5 lead">
            We offer unique service and we also priotize our customers
            comfortability and satisfaction, We believe you deserve the best.
          </p>
          <!-- svelte-ignore a11y-invalid-attribute -->
          <p><a href="#" class="btn btn-primary">Learn More</a></p>
        </div>
      </div>
    </div>
  </div>
</section>
<Promo />
