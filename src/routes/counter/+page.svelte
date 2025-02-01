<script>
  let count = $state(0);
  let isOdd = $derived(count % 2 === 1);
</script>

<button onclick={count++}>The count is {count}</button>

<div class:odd={isOdd}>The number is {isOdd ? "odd" : "even"}.</div>

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

  .odd {
    background: black;
    color: white;
  }
</style>
