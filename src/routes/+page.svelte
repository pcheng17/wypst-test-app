<script>
  import wypst from 'wypst';
  let typst_str = '$1/2 + 1/2 = 1$';
  let rendered = wypst.renderToString(typst_str, { displayMode: false, throwOnError: false });
</script>

{#if rendered}
  <div>{@html rendered}</div>
{:else}
  <div>Something went wrong...</div>
{/if}
