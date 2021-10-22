# Prettier plugin sort imports minimal repro

Reproduce with `npm run prettier`

Before:
```svelte
<script lang="ts">
  import poop from './poop';
  import noop from './noop';

  // Comment one
  let someProp: string = "";

  // Comment two
  let anotherProp: string = "";
</script>

<main />
```

After:
```svelte
<script lang="ts">
  import noop from "./noop";
  import poop from "./poop";
  ';

  // Comme
  let someProp: string = "";
  ";

  // Comme
  let anotherProp: string = "";
</script>

<main />
```
