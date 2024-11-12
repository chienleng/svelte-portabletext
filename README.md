# @eirikk/portabletext-2-svelte-5

A (hopefully temporary) drop-in replacement for [`@portabletext/svelte@2`](https://www.npmjs.com/package/@portabletext/svelte) which works with Svelte 5.

## Setup

I recommend creating an alias in your `package.json` so that you don't need to change all your imports.

If you're sure that only your app and none of your dependencies depends on `@portabletext/svelte` then you can also simply adjust your `dependencies`:

```diff
{
  "dependencies": {
-    "@portabletext/svelte": "^2"
+    "@portabletext/svelte": "npm:@eirikk/portabletext-2-svelte-5@0.1.0-alpha.2"
  }
}
```

Else use you package manager's override mechanism to ensure that dependencies of your app also get the drop-in:

**Using npm (with `overrides` field)**

```json
{
  "overrides": {
    "@portabletext/svelte": "npm:@eirikk/portabletext-2-svelte-5@0.1.0-alpha.2"
  }
}
```

**Using pnpm (with `pnpm.overrides` field)**

```json
{
  "pnpm": {
    "overrides": {
      "@portabletext/svelte": "npm:@eirikk/portabletext-2-svelte-5@0.1.0-alpha.2"
    }
  }
}
```

## Temporary

This intended to be a **temporary** solution until the 1st party package is updated.