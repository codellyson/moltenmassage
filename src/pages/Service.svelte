<script>
  import Hero from "../components/Hero.svelte";
  const services = [
    {
      image: "images/massage.jpg",
      name: "Body Shrub",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 1,
    },
    {
      image: "images/massage2.jpg",
      name: "Outer Home Services",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 2,
    },
    {
      image: "images/testify-1.jpg",
      name: "Santiosage",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 3,
    },
    {
      image: "images/reflex.jpg",
      name: "Reflexology",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/sitting-massage.jpg",
      name: "Nutritional Consultation",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 5,
    },
    {
      image: "images/personal-training.jpg",
      name: "Personal Training",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 6,
    },
    {
      image: "images/volleyball.jpg",
      name: "Private Volleyball Lessons",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 7,
    },
    {
      image: "images/smile-massage.png",
      name: "Deep Massage",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 8,
    },
    {
      image: "images/sitting-massage.jpg",
      name: "Superficial Massage",
      desc:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 9,
    },
    // {
    //   image: "",
    //   name: "In Home Massages",
    //   desc:
    //     "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
    //   id: 10,
    // },
    // {
    //   image: "images/sitting-massage.jpg",
    //   name: "In Home Massages",
    //   desc:
    //     "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
    //   id: 11,
    // },
    // {
    //   image: "images/sitting-massage.jpg",
    //   name: "In Home Massages",
    //   desc:
    //     "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
    //   id: 12,
    // },
  ];
  let pageIntro =
    "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.";
</script>

<svelte:head>
  <title>Service</title>
</svelte:head>
<Hero pageHeading="Our Service" {pageIntro} />
<!-- first -->
<section id="service" class="bg-light">
  <div class="site-section">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2
            class="heading-border-bottom font-weight-bold serif text-black mb-5 text-center"
          >
            Our Services
          </h2>
        </div>
      </div>
      <div class="row" style="justify-content:center">
        {#each services as service}
          <div class="col-lg-3 col-md-6 mb-5 mb-lg-5">
            <div class="service-block">
              <!-- svelte-ignore a11y-img-redundant-alt -->
              <!-- svelte-ignore a11y-invalid-attribute -->
              <a
                href="#"
                class="mb-3 d-block"
                style="display:block; height:200px; overflow:hidden;"
                ><img src={service.image} alt="Image" class="img-fluid" /></a
              >
              <div class="text">
                <h3 class="mb-3">{service.name}</h3>
                <p>{service.desc}</p>
              </div>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
  <!-- Third -->
</section>

<style>
  .service-block {
    background-color: #fff;
  }
  .service-block .text {
    text-align: center;
    padding: 15px 15px;
  }
  .service-block .text h3 {
    font-size: 18px;
  }

  #service {
    padding: 8rem 0;
  }
</style>
