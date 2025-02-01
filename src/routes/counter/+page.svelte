<script>
  let count = $state(0);
</script>

<button onclick={count++}>The count is {count}</button>

<h3>What the code looks like:</h3>

<pre><code>
  &lt;script&gt;
    let count = $state(0);
  &lt;/script&gt;
  
  &lt;button onclick={"{"}count++{"}"}&gt;The count is {"{"}count{"}"}&lt;/button&gt;

  &lt;style&gt;
    button {"{"}
      font-size: 4rem;
    {"}"}
  &lt;/style&gt;
</code></pre>

<style>
  button {
    font-size: 4rem;
  }
</style>
