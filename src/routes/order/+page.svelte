<script lang="ts">
  import { Stepper, Step, SlideToggle } from "@skeletonlabs/skeleton";
  let locked = true;
</script>

<div
  class="w-full p-60 flex flex-col items-center content-center justify-center gap-20"
>
  <div class="w-full card p-4 text-token">
    <Stepper>
      <Step>
        <svelte:fragment slot="header">Get Started!</svelte:fragment>
        <p>
          This example Stepper will teach you how to use this component. Tap <u
            >next</u
          > to proceed to the next step.
        </p>
        <!-- <svelte:fragment slot="navigation"><button class="btn variant-ghost-error">Abort</button></svelte:fragment> -->
      </Step>
      <Step>
        <svelte:fragment slot="header">Going Back.</svelte:fragment>
        <p>
          The current step progress will be tracked at the top. Tap <u>back</u> to
          return to the previous step.
        </p>
      </Step>
      <Step {locked}>
        <svelte:fragment slot="header">A Locked Step.</svelte:fragment>
        <p>
          This Step component uses the <code class="code">locked</code> property
          to prevent progress. This is ideal for multi-step forms, such as registration.
          For now we'll simulate a successful validation condition using the toggle
          below.
        </p>
        <aside class="alert variant-ghost-warning">
          <div class="alert-message">
            <p>This step is <u>{locked ? "Locked" : "Unlocked"}</u></p>
          </div>
          <div class="alert-actions">
            <SlideToggle
              name="locked-state"
              bind:checked={locked}
              active="bg-warning-500"
            />
          </div>
        </aside>
      </Step>
      <Step>
        <svelte:fragment slot="header">Long Form Content.</svelte:fragment>
        <p>The steps will expand to fit content of any length.</p>
        <p>
          <!-- cspell:disable -->
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque vel expedita
          porro vero, saepe dicta repellendus facilis ab accusamus unde, tempora
          ut nobis eum. Veniam, architecto corrupti. Lorem ipsum dolor sit amet consectetur
          adipisicing elit. Itaque vel expedita porro vero, saepe dicta repellendus
          facilis ab accusamus unde, tempora ut nobis eum. Veniam, architecto corrupti.
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque vel expedita
          porro vero, saepe dicta repellendus facilis ab accusamus unde, tempora
          ut nobis eum. Veniam, architecto corrupti. Lorem ipsum dolor sit amet consectetur
          adipisicing elit. Itaque vel expedita porro vero, saepe dicta repellendus
          facilis ab accusamus unde, tempora ut nobis eum. Veniam, architecto corrupti.
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque vel expedita
          porro vero, saepe dicta repellendus facilis ab accusamus unde, tempora
          ut nobis eum. Veniam, architecto corrupti.
          <!-- cspell:enable -->
        </p>
      </Step>
      <Step>
        <svelte:fragment slot="header">Almost Done.</svelte:fragment>
        <p>
          A Complete button will appear on the last step. When the step is
          unlocked and the button pressed, an <code class="code"
            >on:complete</code
          > event will be fired. You can use this trigger to submit form data to
          a server.
        </p>
      </Step>
    </Stepper>
  </div>
</div>
