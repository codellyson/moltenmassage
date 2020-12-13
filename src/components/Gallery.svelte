<script>
  export let gallery;
</script>

<div class="container-fluid">
  <div class="imglist row no-gutters" style="">
    {#each gallery as photo}
      <div class="col-lg-3 col-md-3 ">
        <div class="card" style="border:none;margin:0;">
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
