<script>
  import FeedbackItem from "./FeedbackItem.svelte";
  export let feedback = []; //If not passed in should be an empty array
  console.log(feedback);
</script>

{#each feedback as fb (fb.id)}
  <FeedbackItem item={fb} on:delete-feedback />
{/each}
