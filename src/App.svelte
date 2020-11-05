<script>
  import Navbar from "./components/Navbar.svelte";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  import Service from "./pages/Service.svelte";
  import Contact from "./pages/Contact.svelte";
  import Footer from "./components/Footer.svelte";
  import router from "page";

  let currentPage;
  let pageHeading;
  let pageTitle;

  router("/", () => {
    currentPage = Home;
    pageTitle = "Home";
    // pageHeading = "Spa Which You Love";
  });
  router("/about", () => {
    {
      currentPage = About;
      // pageTitle = "About";
      // pageHeading = "About Us";
    }
  });
  router("/contact", () => {
    {
      currentPage = Contact;
      // pageTitle = "Contact";
      // pageHeading = "Contact Us";
    }
  });
  router("/service", () => {
    currentPage = Service;
    // pageTitle = "Service";
    // pageHeading = "Our Services";
  });
  router.start();
</script>

<style>
</style>

<Navbar />
<main>
  <svelte:component this={currentPage} />
</main>
<Footer />
