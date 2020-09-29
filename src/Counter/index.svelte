<script>
  export let count;

  import styles from "./styles.js";

  function inc() {
    count += 1;
  }

  function dec() {
    if (count !== 0) count -= 1;
  }
</script>

<div class={styles}>
  <button on:click={dec} class="dec"> - </button>
  <span class="count">{count}</span>
  <button on:click={inc} class="inc"> + </button>
</div>
