<script>
  import Navbar from "./components/Navbar.svelte";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  import Service from "./pages/Service.svelte";
  import Contact from "./pages/Contact.svelte";
  import Footer from "./components/Footer.svelte";
  import Spinner from "./components/Spinner.svelte";
  import router from "page";

  let currentPage;
  let segment;
  router("/", () => {
    currentPage = Home;
    segment = undefined;
  });
  router("/about", () => {
    {
      currentPage = About;
      segment = "about";
    }
  });
  router("/contact", () => {
    {
      currentPage = Contact;
      segment = "contact";
    }
  });
  router("/service", () => {
    currentPage = Service;
    segment = "service";
  });
  router.start({ hashbang: true });
</script>

<style>
  main {
    overflow: hidden;
  }
</style>

<Navbar {segment} />
<main>
  <Spinner loading="true" />
  <svelte:component this={currentPage} />
</main>
<Footer />
