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
  });
  router("/about", () => {
    {
      currentPage = About;
    }
  });
  router("/contact", () => {
    {
      currentPage = Contact;
    }
  });
  router("/service", () => {
    currentPage = Service;
  });
  router.start({ hashbang: true });
</script>

<style>
</style>

<Navbar />
<main>
  <svelte:component this={currentPage} />
</main>
<Footer />
