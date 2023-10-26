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
        <svelte:fragment slot="header">Order Cookie Mixes</svelte:fragment>
        <p>
          Welcome to our cookie mix ordering process. Tap <u>next</u> to proceed to the next step.
        </p>
      </Step>
      <Step>
        <svelte:fragment slot="header">Choose Your Mixes</svelte:fragment>
        <p>
          Please select the cookie mixes you would like to order. Tap <u>back</u> to return to the previous step.
        </p>
        <ul>
          <li>Chocolate Chip Cookie Mix</li>
          <li>Oatmeal Raisin Cookie Mix</li>
          <li>Sugar Cookie Mix</li>
        </ul>
      </Step>
      <Step {locked}>
        <svelte:fragment slot="header">Confirm Your Order</svelte:fragment>
        <p>
          Please review your order and confirm that it is correct. For now we'll simulate a successful validation condition using the toggle below.
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
        <svelte:fragment slot="header">Provide Your Information</svelte:fragment>
        <p>Please provide your contact and shipping information so we can process your order.</p>
        <form>
          <label for="name">Name:</label>
          <input type="text" id="name" name="name"><br><br>
          <label for="email">Email:</label>
          <input type="email" id="email" name="email"><br><br>
          <label for="address">Address:</label>
          <input type="text" id="address" name="address"><br><br>
          <label for="city">City:</label>
          <input type="text" id="city" name="city"><br><br>
          <label for="state">State:</label>
          <input type="text" id="state" name="state"><br><br>
          <label for="zip">Zip Code:</label>
          <input type="text" id="zip" name="zip"><br><br>
        </form>
      </Step>
      <Step>
        <svelte:fragment slot="header">Complete Your Order</svelte:fragment>
        <p>
          Please review your order information and tap the <u>Complete Order</u> button to submit your order.
        </p>
        <button class="btn variant-primary" on:click={() => alert("Order submitted!")}>Complete Order</button>
      </Step>
    </Stepper>
  </div>
</div>
