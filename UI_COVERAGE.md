# UI Coverage (Progress: 26/26)
Legend: [ ] not yet tested  -  [x] test written and passing  -  [~] intentionally skipped (reason)

## Core Navigation
- [x] /page-1.html — basic Swup navigation, data-testid links, API navigate, title updates (`navigation.spec.ts`)
- [x] /page-2.html — navigation target, heading/title verification (`navigation.spec.ts`)
- [x] /page-3.html — navigation target, heading/title verification (`navigation.spec.ts`)
- [x] /instance.html — minimal Swup init, API surface, destroy hook (`instance.spec.ts`)
- [x] /link-resolution.html — absolute/relative/self/external links (`link-resolution.spec.ts`)
- [x] /nested/nested-1.html + nested-2.html — base-href relative link resolution, manual Swup init (`link-resolution.spec.ts`)
- [x] /link-selector.html — SVG anchor via Swup, imagemap area href verified (`link-selector.spec.ts`)

## Animation
- [x] /animation-duration.html — 400 ms opacity transition timing (`animation-timing.spec.ts`)
- [x] /animation-complex.html — 600 ms multi-property timing (`animation-timing.spec.ts`)
- [x] /animation-keyframes.html — 700 ms keyframe + delay timing (`animation-timing.spec.ts`)
- [x] /animation-none.html — transition:none, instant nav, hooks fire (`animation-extra.spec.ts`)
- [x] /animation-partial.html — only #swup container animated (`animation-extra.spec.ts`)
- [x] /animation-duration.html (class lifecycle) — is-changing/is-animating/is-leaving/is-rendering lifecycle (`animation-classes.spec.ts`)
- [x] /animation-native.html — native:true option, View Transitions API (`native-mode.spec.ts`)

## Instance & Lifecycle
- [x] /instance.html — swup-enabled, destroy, disable hook, default options, empty cache (`instance.spec.ts`)

## Caching
- [x] /page-1.html (cache) — cache populated after nav, disable per-nav via cache:{read/write}, clear programmatically (`cache.spec.ts`)

## History
- [x] /history.html — pushState vs replaceState (data-swup-history="replace"), back navigation, popstate (`history.spec.ts`)

## Scrolling
- [x] /scrolling-1.html + /scrolling-2.html — cross-page anchor scroll, top scroll, same-page hash (`scrolling.spec.ts`)

## Special Visit Handling
- [x] /ignore-visits.html — data-no-swup on link/parent triggers full reload, normal link uses Swup (`ignore-visits.spec.ts`)
- [x] /containers-1.html + /containers-2.html — both #main and #aside containers updated on nav (`containers.spec.ts`)
- [x] /persist-1.html + /persist-2.html — data-swup-persist keeps element text across nav (`persist.spec.ts`)
- [x] /redirect-1/2/3.html — server 301 redirect followed, redirected pages not cached (`redirects.spec.ts`)

## Rapid Navigation
- [x] /rapid-navigation/page-1/2/3.html — cache:false, aria-busy lifecycle, hook capture in window.data (`rapid-navigation.spec.ts`)

## Integrations
- [x] /alpinejs/page-1/2.html — swup:link:click → click-fired class, swup:any → any-fired class (`alpinejs.spec.ts`)
- [x] /plugins/body-class-plugin/page-1/2.html — body class updated (body-1↔body-2) on navigation (`plugins/body-class-plugin.spec.ts`)
- [x] /plugins/scroll-plugin/page-1/2.html — scroll to anchor/top, cross-page anchor scroll (`plugins/scroll-plugin.spec.ts`)
