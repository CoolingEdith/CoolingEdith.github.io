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
          MyMix UF är ett UF-företag som tagit fram en kakmix med fokus på att det ska vara lätt för alla att kunna
         baka oavsett vem du är eller var du är. Vårt mål är att alla ska kunna baka!
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
          ><p class="font-bold">Vilka är vi?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
            Vi är 4 elever från Umeå Elitidrottsgymnasium:<br>
            Emmy Erlandsson - Prduktansvarig, marknadsförare<br>
            Edith Lindström - Webbmaster, marknadsförare<br>
            Gustav Ydreborg - Webbmaster<br>
            Gustav Ekros - Ekonomiansvarig
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
          ><p class="font-bold">Hur länge säljer vi?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          Vi startade vår försäljning 26-11-23 och kommer sälja till 31-05-24
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
          ><p class="font-bold">Vad innehåller kakmixen?</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
          Ingridienser: <br>
          Vetemjöl, Farinsocker, Choklad*, Strösocker, Vaniljsocker, Majsstärkelse, Bikarbonat<br>
          *Chokladens ingridienser "www.lyckasmedmat.se": <br>
          Kakaomassa, socker, kakaosmör,emulgeringsmedel:SOJALECITIN, naturlig vaniljsmak. Kosher. Kan innhålla MJÖLK.
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
          ><p class="font-bold">Kontakta oss</p></svelte:fragment
        >
        <svelte:fragment slot="content">
          <!-- prettier-ignore -->
          <p>
            <a target="_blank" href="https://www.instagram.com/mymixuf/">Instagram: @mymixuf</a> <br>
            <a target="_blank" href="https://www.tiktok.com/@mymixuf?ug_source=op.auth&ug_term=Linktr.ee&utm_source=awyc6vc625ejxp86&utm_campaign=tt4d_profile_link&_r=1">Tiktok: @mymixuf</a>
            <br>Mail: mymixuf@hotmail.com
          </p>
        </svelte:fragment>
      </AccordionItem>
    </Accordion>
  </div>
</div>

