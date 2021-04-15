<script>
  const teams = [
    {
      image: "images/founder.jpg",
      name: "Donovan Buckle",
      post: "Director",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork ",
      id: 1,
    },
    {
      image: "images/founder.jpg",
      name: "Donovan Buckle",
      post: "Director",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork ",
      id: 2,
    },
    {
      image: "images/founder.jpg",
      name: "Donovan Buckle",
      post: "Director",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork ",
      id: 3,
    },
    {
      image: "images/founder.jpg",
      name: "Donovan Buckle",
      post: "Director",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork ",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Donovan Buckle",
      post: "Director",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork ",
      id: 5,
    },
    {
      image: "images/founder.jpg",
      name: "Donovan Buckle",
      post: "Director",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork ",
      id: 6,
    },
  ];
  const gallery = [
    {
      image: "images/founder.jpg",
      caption: "caption here",
      id: 1,
    },
    {
      image: "images/volleyball.jpg",
      caption: "caption here",
      id: 2,
    },
    {
      image: "images/leg-massage.jpg",
      caption: "caption here",
      id: 3,
    },

    {
      image: "images/massage2.jpg",
      caption: "caption here",
      id: 5,
    },
    {
      image: "images/indoor.jpg",
      caption: "caption here",
      id: 6,
    },
    {
      image: "images/massage-dev.jpg",
      caption: "caption here",
      id: 7,
    },
    {
      image: "images/plenty-people2.jpg",
      caption: "caption here",
      id: 8,
    },
    {
      image: "images/reflex.jpg",
      caption: "caption here",
      id: 9,
    },
    {
      image: "images/sitting-massage.jpg",
      caption: "caption here",
      id: 10,
    },
    {
      image: "images/smile-massage.png",
      caption: "caption here",
      id: 11,
    },
    {
      image: "images/testify-1.jpg",
      caption: "caption here",
      id: 12,
    },
    {
      image: "images/press-phone.jpg",
      caption: "caption here",
      id: 13,
    },
    {
      image: "images/regcenter.jpg",
      caption: "caption here",
      id: 14,
    },
    {
      image: "images/ncaa.jpg",
      caption: "caption here",
      id: 15,
    },
  ];

  import Hero from "../components/Hero.svelte";
  import Gallery from "../components/Gallery.svelte";
  let pageIntro =
    "Our mission is to promote relaxation, stress relief, and a pain free lifestyle through therapeutic massage and bodywork, while supporting you in healing yourself holistically.";
</script>

<svelte:head>
  <title>About</title>
</svelte:head>
<Hero pageHeading="About Us" {pageIntro} />
<section id="about">
  <div class="site-section py-5 my-5">
    <h1 class="section-header-text text-center py-3">About Us</h1>
    <div class="container">
      <div class="row align-items-center">
        <div class="col-md-5 mr-auto mb-5">
          <h2 class="serif font-weight-bold mb-3">Molten Massage Int'l</h2>
          <p class="font-weight-bold">
            Our mission is to promote relaxation, stress relief, and a pain free
            lifestyle through therapeutic massage and bodywork, while supporting
            you in healing yourself holistically.
          </p>
          <p>
            MMI's focus is to provide natural solutions to you the client, as
            well as education that ultimately result in helping you realize
            optimal, physical and physiological health and happiness.
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
              style="background-image:url(../images/green-plant.jpg"
            />
            <div
              class="bg-img-1"
              style="background-image:url(../images/green-plant.jpg)"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- Gallery -->
  <section id="gallery" class="py-5 my-5">
    <div class="">
      <div class="row">
        <div class="col-12">
          <h2 class="section-header-text text-black mb-2 text-center">
            Gallery
          </h2>
        </div>
      </div>
      <p class="text-center py-2">A look into what we do</p>
      <Gallery {gallery} />
    </div>
  </section>

  <!-- Side Two -->
  <div class="site-section bg-light">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2 class="section-header-text text-black mb-2 text-center">
            Our Team
          </h2>
        </div>
      </div>
      <div class="row align-items-stretch">
        {#each teams as team}
          <div class="col-lg-4 col-md-6 mb-5">
            <div
              class="team_card h-100 person-1 aos-init aos-animate"
              data-aos="fade-up"
              data-aos-delay="{team.id}00"
            >
              <!-- svelte-ignore a11y-img-redundant-alt -->
              <img src={team.image} alt="Image" class="img-fluid" />
              <div class="team_card-contents ">
                <span class="meta">{team.post}</span>
                <h2 class="my-2">{team.name}</h2>
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
            data-aos="fade-up"
            data-aos-delay="400"
          >
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src="images/green-plant.jpg" alt="Image" class="img-fluid" />
          </div>
        </div>
        <div
          class="col-lg-5 ml-auto pl-lg-5 text-center aos-init aos-animate"
          data-aos="fade-down"
          data-aos-delay="400"
        >
          <h2
            class="heading-border-bottom font-weight-bold serif text-black mb-5 text-center"
          >
            Why Us
          </h2>
          <p class="mb-5 lead">
            We offer unique services and we also priotize our customers
            comfortability and satisfaction, We believe you deserve the best.
          </p>
          <!-- svelte-ignore a11y-invalid-attribute -->
          <p><a href="/service" class="btn btn-primary">Learn More</a></p>
        </div>
      </div>
    </div>
  </div>
</section>

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
  .team_card.person-1 .team_card-contents {
    padding-top: 4rem;
  }
  .team_card .team_card-contents {
    background: #ffa288;
    color: #fff;
    padding: 20px;
  }
  .team_card.person-1 {
    text-align: center;
  }
  .team_card.person-1 img {
    width: 90px;
    border-radius: 50%;
    margin: 0 auto -45px auto;
    border: 10px solid #fff;
  }
  .team_card .meta {
    color: #ffa288;
    background: #fff;
    padding: 0.5rem;
    border-radius: 8px;
  }

  .team_card .team_card-contents h2 {
    font-size: 22px;
    margin-bottom: 20px;
  }
  p {
    margin-top: 0;
    margin-bottom: 1rem;
  }
</style>
