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
          ><p class="font-bold">What is Día de los Muertos?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          While Halloween and Day of the Dead occur nearly in tandem and share similar customs (candy, face painting, and community gathering), the two are not related. Halloween has ancient Celtic roots, while Day of the Dead has its own origins that date back to the Indigenous people of Mexico and Central America.
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
          ><p class="font-bold">When did it begin?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          Roughly 3000 years ago, amongst the Aztec, Toltec, and Mayans, death and the dead were seen as a natural part of life that should be honored and celebrated, rather than mourned. In particular, the Nahua people of central Mexico believed the deceased traveled on a years-long journey to Chicunamictlán, the Land of the Dead. The living would provide supplies, such as food and water to aid them on the trek. This practice inspired the modern tradition of creating altars —known as ofrendas— at their homes, in addition to leaving offerings at the gravesites of loved ones.
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
