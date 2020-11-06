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
  let active = false;

  router("/", () => {
    currentPage = Home;
    active = true;
  });
  router("/about", () => {
    {
      currentPage = About;
      active = true;
    }
  });
  router("/contact", () => {
    {
      currentPage = Contact;
      active = true;
    }
  });
  router("/service", () => {
    currentPage = Service;
  });
  router.start({ hashbang: true });
</script>

<style>
</style>

<Navbar {active} />
<main>
  <svelte:component this={currentPage} />
</main>
<Footer />
