<script lang="ts">
  const images = [
    [
      "UF-ugn2.png",
      "UF-rörihop.png",
      "UF-kyl.png",
    ],
    [
      "UF-smör.png",
      "UF-vatten.png",
      "UF-plåt.png",
    ],
    [
      "UF-mixen.png",
      "UF-rulla.png",
      "UF-ugn.png",,
    ],
  ];
</script>

<section class="p-20 grid grid-cols-2 md:grid-cols-4 gap-2">
  {#each images as imageGroup}
    <div class="grid gap-4">
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
  }

  img:hover {
    transform: scale(1.05);
  }
</style>
