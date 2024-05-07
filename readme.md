# qwik-typescript-js-extension-issue

This repository demonstrates the issue when building Qwik app if there's the `.js` extension in module's path

## Reproduction

1. Clone this repository via `git clone git@github.com:octet-stream/qwik-typescript-js-extension-issue.git`
2. Install dependencies with `pnpm i`
3. Run `pnpm build` and you'll get following error message

```
vite v5.2.11 building for production...
✓ 44 modules transformed.
x Build failed in 86ms
error during build:
RollupError: Could not resolve "./components/router-head/router-head.js" from "src/s_tntnak2dhj8.js"
file: /Users/octetstream/projects/qwik-test/src/s_tntnak2dhj8.js
    at getRollupError (file:///Users/octetstream/projects/qwik-test/node_modules/.pnpm/rollup@4.17.2/node_modules/rollup/dist/es/shared/parseAst.js:394:41)
    at error (file:///Users/octetstream/projects/qwik-test/node_modules/.pnpm/rollup@4.17.2/node_modules/rollup/dist/es/shared/parseAst.js:390:42)
    at ModuleLoader.handleInvalidResolvedId (file:///Users/octetstream/projects/qwik-test/node_modules/.pnpm/rollup@4.17.2/node_modules/rollup/dist/es/shared/node-entry.js:19106:24)
    at file:///Users/octetstream/projects/qwik-test/node_modules/.pnpm/rollup@4.17.2/node_modules/rollup/dist/es/shared/node-entry.js:19066:26
 ELIFECYCLE  Command failed with exit code 1.
 ELIFECYCLE  Command failed with exit code 1.
 ELIFECYCLE  Command failed.
```
