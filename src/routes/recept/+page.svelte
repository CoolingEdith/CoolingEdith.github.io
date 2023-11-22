<br>
<h1>Såhär gör du:</h1><br>

<script lang="ts">
  const images = [
    [
      "UF-smör.png",
      "UF-mixen.png",
      "UF-vatten.png",
      "UF-blanda.png",
      "UF-kyl.png",
      "UF-ugn2.png",
      "UF-rulla.png",
      "UF-plåt.png",
      "UF-ugn.png",
    ]
  ]
</script>

<section class="p-10 grid grid-cols-2 md:grid-cols-4 gap-2">
  {#each images as imageGroup}
    <div class="grid gap-40">
      {#each imageGroup as imgUrl}
        <div>
          <img class="h-auto max-w-full rounded-lg" src={imgUrl} alt="" />
        </div>
      {/each}
    </div>
  {/each}
</section>

<style>
  img {
    transition: all 0.2s;
    transform: scale(1.2);
  }

  img:hover {
    transform: scale(1.23);
  }



  h1 {
    color: rgb(0, 174, 254);
    font-size: xx-large;
  }
  

</style>
