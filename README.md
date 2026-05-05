# qa-practice-vue

A viiibin **practice repo**. Bare Vue 3 + Vite + TypeScript scaffold paired
with a [`SPEC.md`](./SPEC.md) describing exactly what the agent should build.

## Use it

1. Open viiibin → New Project → Import from GitHub
2. Paste: `https://github.com/iii-Partners/qa-practice-vue`
3. Once the workspace loads, ask the agent: **"Read SPEC.md and build it."**
4. Watch the preview update with the implemented feature.

## What you get

- Vue 3 (Composition API) + Vite + TypeScript (strict)
- Dev server bound to `0.0.0.0:3000` (so viiibin's preview proxy finds it)
- A clean `App.vue` placeholder — empty `<main />`, no demo content
- A standard `SPEC.md` with strict, parseable acceptance criteria

## Why "practice"?

This repo is part of viiibin's framework validation matrix
([milestone M57](https://github.com/iii-Partners/viiibin/milestone/103)).
The same SPEC across nine framework variants — React, Next.js, Astro, Vue,
Nuxt, Svelte/Kit, Remix, Angular — proves the platform handles each one
end-to-end. The repos are also a clean starting point for anyone evaluating
viiibin.

## Local sanity check

```bash
npm install
npm run dev    # http://localhost:3000
npm run build  # → dist/
```

## Framework notes

- The Vite-family prep path in viiibin's sandbox detects `vite.config.ts` and
  launches the dev server directly via `npx vite --host 0.0.0.0 --port 3000`,
  so the binding is reliable across SDK versions.
- Use Vue's standard `<script setup lang="ts">` SFC pattern for new
  components. No router, no Pinia, no devtools plugin — the scaffold is
  intentionally minimal so the agent has a clean canvas.

## License

MIT — see [LICENSE](./LICENSE).
