<script>
  import {createEventDispatcher, onMount} from "svelte"
  const dispatch = createEventDispatcher();

  /**
   * Must be `trigger` value
   * @type Function
   */
  export let trigger

  onMount(() => {
    dispatch(trigger());
  });

</script>
