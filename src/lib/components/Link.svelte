<script lang="ts">
  import { twMerge } from 'tailwind-merge';

  let klass: string | null = null;

  export let href: string;
  export { klass as class };
</script>

<a
  class={twMerge(
    'rounded-full border border-zinc-700 bg-zinc-800 p-2 text-zinc-500 hover:bg-zinc-700 hover:text-zinc-400 hover:transition-colors hover:duration-300',
    klass
  )}
  {href}
  target="_blank"
>
  <slot />
</a>
