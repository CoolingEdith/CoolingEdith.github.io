<script lang="ts">
  const images = [
    [
      "UF-mixen.png",
      "UF-kyl.png",
      "UF-plåt.png",
    ],
    [
      "UF-rörihop.png",
      "UF-rulla.png",
      "UF-smör.png",
    ],
    [
      "UF-ugn.png",
      "UF-ugn2.png",
      "UF-vatten.png",
    ],
    [
      "https://images.unsplash.com/photo-1633053663400-655b31fb88ac?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY4MDV8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max",
      "https://images.unsplash.com/photo-1578170222009-c7893aa20afd?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY4MTZ8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max",
      "https://images.unsplash.com/photo-1610220941077-1ec123e7c043?ixid=M3w0Njc5ODF8MHwxfGFsbHx8fHx8fHx8fDE2ODc5NzY4NjV8&ixlib=rb-4.0.3&w=300&h=300&auto=format&fit=max",
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
