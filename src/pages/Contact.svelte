<script>
  import Hero from "../components/Hero.svelte";
  let pageIntro =
    "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.";
</script>

<svelte:head>
  <title>Contact</title>
</svelte:head>
<Hero pageHeading="Contact Us" {pageIntro} />
<section id="contact" class="contact section-bg bg-light ">
  <div class="container ">
    <div class="section-title mb-5">
      <h2
        data-aos="fade-in"
        class="aos-init aos-animate text-center section-header-text "
      >
        Contact
      </h2>
      <p data-aos="fade-in" class="aos-init aos-animate text-center ">
        You can reach out to us with one of the options below
      </p>
    </div>

    <div class="row">
      <div class="col-lg-6">
        <div class="row">
          <div class="col-md-12">
            <div class="info-box aos-init aos-animate " data-aos="fade-up">
              <i class="icon-map-marker text-primary" />
              <h3>Address</h3>
              <p>Ican American: *477 East 96 Street Brooklyn, NY 11212</p>
            </div>
          </div>
          <div class="col-md-6">
            <div
              class="info-box mt-4 aos-init aos-animate "
              data-aos="fade-up"
              data-aos-delay="100"
            >
              <i class="icon-envelope text-primary" />
              <h3 class="">Email Us</h3>
              <p>buckleballa41@gmail.com</p>
            </div>
          </div>
          <div class="col-md-6">
            <div
              class="info-box mt-4 aos-init aos-animate "
              data-aos="fade-up"
              data-aos-delay="100"
            >
              <i class="icon-phone text-primary" />
              <h3 class="">Call Us</h3>
              <p>(718)600-3298</p>
            </div>
          </div>
        </div>
      </div>

      <div class="col-lg-6">
        <form
          action="forms/contact.php"
          method="post"
          role="form"
          class="php-email-form aos-init aos-animate"
          data-aos="fade-up"
        >
          <div class="form-row">
            <div class="col-md-6 form-group">
              <input
                type="text"
                name="name"
                class="form-control"
                id="name"
                placeholder="Your Name"
                data-rule="minlen:4"
                data-msg="Please enter at least 4 chars"
              />
              <div class="validate" />
            </div>
            <div class="col-md-6 form-group">
              <input
                type="email"
                class="form-control"
                name="email"
                id="email"
                placeholder="Your Email"
                data-rule="email"
                data-msg="Please enter a valid email"
              />
              <div class="validate" />
            </div>
          </div>
          <div class="form-group">
            <input
              type="text"
              class="form-control"
              name="subject"
              id="subject"
              placeholder="Subject"
              data-rule="minlen:4"
              data-msg="Please enter at least 8 chars of subject"
            />
            <div class="validate" />
          </div>
          <div class="form-group">
            <textarea
              class="form-control"
              name="message"
              rows="5"
              data-rule="required"
              data-msg="Please write something for us"
              placeholder="Message"
            />
            <div class="validate" />
          </div>

          <div class="text-center">
            <button type="submit " class="btn btn-primary">Send Message</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</section>

<style>
  input.form-control {
    display: block;
    width: 100%;
    padding: 1.5rem;
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.5;
    color: #495057;
    height: 55px;
    background: #fff !important;
  }
  input:focus,
  textarea:focus {
    outline: #495057 !important;
    border-color: #495057;
  }
  #contact {
    padding: 8rem 0;
  }
  #contact i {
    display: block;
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }

  /* .contact-icon . */
</style>
