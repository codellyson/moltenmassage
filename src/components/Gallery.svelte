<script>
  export let gallery;
</script>

<style>
  .gallery-img {
    position: relative;
  }
  .gallery-img-card:hover ~ .gallery-img-card::before {
    content: "Open Image";
    display: block;
    height: 100%;
    width: 100%;
    background-color: rgba(0, 0, 0, 0.445);
    position: absolute;
    z-index: 1;
    top: 0;
    right: 0;
  }
</style>

<div class="container-fluid">
  <div class="imglist row no-gutters" style="">
    {#each gallery as photo}
      <div class="col-lg-3 col-md-3 gallery-img">
        <div class="card gallery-img-card" style="border:none;margin:0;">
          <a
            href={photo.image}
            data-fancybox="images"
            data-caption={photo.caption}>
            <!-- svelte-ignore a11y-missing-attribute -->
            <img
              src={photo.image}
              class="aos-init aos-animate"
              style="height:400px; width:100%;"
              data-aos="fade-up"
              data-aos-delay="{photo.id}00" />
          </a>
        </div>
      </div>
    {/each}
  </div>
</div>
