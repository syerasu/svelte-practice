<script>
  import Scroller from '../lib/Scroller.svelte'
  import ArticleText from '../lib/ArticleText.svelte'
</script>

<Scroller layout="left">
  {#snippet sticky()}
    <h2>This stays still</h2>
  {/snippet}

  {#snippet scrolly()}
    <ArticleText>
      <p>This scrolls into view.</p>
    </ArticleText>

    <ArticleText>
      <p>Here’s more scrolling content.</p>
    </ArticleText>

    <ArticleText>
      <p>Add as many blocks as you want!</p>
    </ArticleText>
  {/snippet}
</Scroller>