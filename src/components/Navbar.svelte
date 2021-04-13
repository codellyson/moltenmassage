<script>
  export let showNav = false;

  const toggleNav = () => {
    showNav === true ? (showNav = false) : (showNav = true);
    // showNav === true ? (showNav = false) : (showNav = true);
  };
  export const activeClass = false;
  // console.log(active);
  export let segment;
</script>

<header id="header">
  <div class="container">
    <nav class="navbar navbar-expand-lg ">
      <a class="navbar-brand" href="/"
        ><img src="images/moltenmassage.png" style="width:100%;" alt="" /></a
      >
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon" />
      </button>
      <div class="mobile-nav-toggler">
        <svg viewBox="0 0 100 80" width="40" height="22" on:click={toggleNav}>
          <rect width="80" height="10" rx="8" />
          <rect y="30" width="70" height="10" rx="8" />
          <rect y="60" width="65" height="10" rx="8" />
        </svg>
      </div>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item active">
            <a href="/" class="nav-link" class:current={segment === undefined}>
              Home</a
            >
          </li>
          <li class="nav-item">
            <a
              href="/about"
              class="nav-link"
              class:current={segment === "about"}
            >
              About</a
            >
          </li>
          <li class="nav-item">
            <a
              href="/service"
              class="nav-link"
              class:current={segment === "service"}
            >
              Service</a
            >
          </li>
          <li class="nav-item">
            <a
              href="/contact"
              class="nav-link"
              class:current={segment === "contact"}
            >
              Contact</a
            >
          </li>
        </ul>
      </div>
      <div class="mobile-nav" class:showNav id="navbarSupportedContent">
        <div class="cancel" on:click={toggleNav}>
          <svg
            className="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
            ><path
              strokeLinecap="round"
              strokeLinejoin="round"
              strokeWidth={2}
              d="M6 18L18 6M6 6l12 12"
            /></svg
          >
        </div>
        <ul class="mobile-nav-menu ml-auto">
          <li
            class="nav-item active"
            data-aos="fade-left"
            data-aos-duration="500"
          >
            <a
              href="/"
              class="nav-link"
              class:current={segment === undefined}
              on:click={toggleNav}
            >
              Home</a
            >
          </li>
          <li
            class="nav-item"
            data-aos="fade-left"
            data-aos-anchor="#example-anchor2"
            data-aos-duration="900"
          >
            <a
              href="/about"
              class="nav-link"
              class:current={segment === "about"}
              on:click={toggleNav}
            >
              About</a
            >
          </li>
          <li class="nav-item" data-aos="fade-left" data-aos-duration="1000">
            <a
              href="/service"
              class="nav-link"
              class:current={segment === "service"}
              on:click={toggleNav}
            >
              Service</a
            >
          </li>
          <li class="nav-item" data-aos="fade-left" data-aos-duration="1200">
            <a
              href="/contact"
              class="nav-link"
              class:current={segment === "contact"}
              on:click={toggleNav}
            >
              Contact</a
            >
          </li>
        </ul>
      </div>
    </nav>

    <!-- .nav-menu  -->
  </div>
</header>

<!-- <div class="container">
  <div class="navbar">
    <div class="menu">
      <h3 />
    </div>
  </div>
</div> -->
<style>
  #header {
    margin-bottom: 0px;
    z-index: 1999;
    position: absolute;
    top: 0;
    width: 100%;
    padding: 1rem;
  }
  li > a {
    margin-left: 15px;
    margin-right: 20px;
    padding: 20px 0;
    color: #fff !important;
    display: inline-block;
    text-decoration: none !important;
  }

  .nav-link {
    font-family: "Open Sans", sans-serif;
    color: #ffffff;
    transition: all 300ms;
    font-size: 1.2rem;
  }
  .nav-link:hover {
    color: #ff9375;
  }
  .nav-item a:hover {
    color: #ff9375 !important;
    /* padding: 0.5rem 0.5rem; */
  }
  .navbar-brand {
    font-size: 1.5rem;
    font-weight: bold;
    font-family: "Playfair Display";
    color: #ffffff;
  }
  .mobile-nav {
    position: fixed;
    height: 100vh;
    background: #000000;
    z-index: -9999999;
    width: 100%;
    visibility: hidden;
    right: 0;
    height: 89.5vh;
    top: 0;
  }
  .mobile-nav ul {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
    list-style: none;
    margin: 6rem 4rem;
    text-align: center;
  }
  .mobile-nav ul li {
    font-size: 1.2rem;
    font-weight: bolder;
    width: 100%;
  }
  .mobile-nav ul li a {
    font-family: "Open Sans", sans-serif;
  }

  .mobile-nav ul li a:hover {
    color: #fa7a56 !important;
  }
  a.current {
    color: #fa7a56 !important;
  }
  .mobile-nav.showNav {
    visibility: visible;
    z-index: 9999999;
  }
  .navbar-toggler,
  .mobile-nav,
  .mobile-nav-toggler {
    display: none;
  }

  .mobile-nav-toggler svg {
    fill: #fff;
  }
  svg {
    color: #fff;
  }

  .cancel {
    width: 34px;
    float: right;
    margin: 1rem;
    font-size: 2.9rem;
    font-weight: 800;
  }
  @media (max-width: 990px) {
    .mobile-nav-toggler {
      display: block;
    }
    .mobile-nav {
      display: initial;
    }
  }
  /* Special style for navbar misbehaviour */
  .navbar-brand {
    width: 50%;
  }
  @media (min-width: 768px) {
    .navbar-brand {
      width: 25%;
    }
    .site-section-cover h1 {
      font-size: 3rem;
    }
  }
</style>
