<script lang="ts">
  import { Accordion, AccordionItem } from "@skeletonlabs/skeleton";
</script>

<div
  class="w-full p-60 flex flex-col items-center content-center justify-center gap-20"
>
  <div class="w-full card p-4 text-token">
    <Accordion autocollapse>
      <AccordionItem open>
        <svelte:fragment slot="lead"
          ><i
            class="fa-solid fa-skull text-xl w-6 text-center"
          /></svelte:fragment
        >
        <svelte:fragment slot="summary"
          ><p class="font-bold">Vad är MyMix UF?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          MyMix UF är ett UF företag som fokuserar på att ta fram en kakmix som ska göra det lätt för alla att kunna baka oavsett vem du är eller var du är.
        </p>
        </svelte:fragment>
      </AccordionItem>
      <AccordionItem>
        <svelte:fragment slot="lead"
          ><i
            class="fa-solid fa-clock text-xl w-6 text-center"
          /></svelte:fragment
        >
        <svelte:fragment slot="summary"
          ><p class="font-bold">Vilka är vi som har MyMix UF?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
            
        </p>
        </svelte:fragment>
      </AccordionItem>
      <AccordionItem>
        <svelte:fragment slot="lead"
          ><i
            class="fa-solid fa-calendar text-xl w-6 text-center"
          /></svelte:fragment
        >
        <svelte:fragment slot="summary"
          ><p class="font-bold">When is it celebrated?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          Once the Spanish colonized Mexico in the 16th century, their own Catholic views on the dead influenced Mexican customs. Día de los Muertos was originally celebrated in the summer months. The holiday came to fall on November 1 and November 2 to align with All Saints Day and All Souls Day.
        </p>
        </svelte:fragment>
      </AccordionItem>
      <AccordionItem>
        <svelte:fragment slot="lead"
          ><i
            class="fa-solid fa-gift text-xl w-6 text-center"
          /></svelte:fragment
        >
        <svelte:fragment slot="summary"
          ><p class="font-bold">What are ofrendas?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          To beckon spirits back into the Land of the Living for the festivities, revelers create makeshift altars, or ofrendas, at their homes and at the gravesites of their deceased loved ones. Families gather at the site to eat, tell stories, and even clean the graves.
        </p>
        </svelte:fragment>
      </AccordionItem>
    </Accordion>
  </div>
</div>
