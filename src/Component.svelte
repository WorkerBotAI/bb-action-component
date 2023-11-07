<script>
  import { createEventDispatcher } from "svelte";
  const dispatch = createEventDispatcher();

  /**
   * Must be `trigger` value
   * @type Function | undefined
   */
  export let trigger;
  trigger && dispatch(trigger?.());
</script>
