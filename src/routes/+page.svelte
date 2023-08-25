<script lang="ts">
  import Link from '@/components/Link.svelte';
  import { Github, Twitter } from '@steeze-ui/lucide-icons';
  import { Icon } from '@steeze-ui/svelte-icon';
  import SvelteSeo from 'svelte-seo';
</script>

<SvelteSeo
  title="kyuu.dev"
  description="Personal website of Kyuu aka kyuuaria."
  openGraph={{
    type: 'website',
    site_name: 'Kyuu',
    url: 'https://kyuu.dev/',
    title: 'kyuu.dev',
    description: 'Personal website of Kyuu aka kyuuaria.',
    images: [{ url: 'https://kyuu.dev/meta.png', width: 1200, height: 630 }]
  }}
  twitter={{
    card: 'summary_large_image',
    title: 'kyuu.dev',
    description: 'Personal website of Kyuu aka kyuuaria.',
    image: 'https://kyuu.dev/meta.png'
  }}
/>

<div class="fixed top-10 flex w-full items-center justify-center">
  <div
    class="mx-4 flex items-center justify-center gap-4 rounded-xl border border-zinc-800 px-4 py-3.5 shadow-2xl shadow-zinc-800 backdrop-blur-sm"
  >
    <Link href="https://github.com/kyuuaria">
      <Icon src={Github} size="16" />
    </Link>
    <Link href="https://twitter.com/kyuuaria">
      <Icon src={Twitter} size="16" />
    </Link>
    <div class="h-7 border-l border-l-zinc-700" />
    <Link
      href="https://discordapp.com/users/652810281654812672"
      class="rounded-xl px-3 py-1 text-center leading-5"
    >
      <span class="font-medium">kyuu.dev</span> on Discord
    </Link>
  </div>
</div>

<div class="flex h-screen flex-col items-center justify-center gap-4 px-12 py-6">
  <h1
    class="font-mono text-3xl font-semibold text-white"
    style="text-shadow: 0 0 15px rgba(255,255,255,.5), 0 0 10px rgba(255,255,255,.5);"
  >
    kyuu.dev
  </h1>
  <p class="text-center text-zinc-300">
    Hey there, my name is <span class="font-medium">Kyuu</span> also known as
    <span class="font-medium">kyuuaria</span>!
  </p>
  <p class="mt-2 rounded-lg border border-zinc-700 bg-zinc-800 px-2 py-0.5 text-xs text-zinc-400">
    IPA /kiːju/
  </p>
</div>
