# UI Coverage (Progress: 28/28)
Legend: [ ] not yet tested  -  [x] test written and passing  -  [~] intentionally skipped (reason)

## Core Navigation
- [x] page-1/2/3 navigation — basic SPA link navigation, nav-bar links, data-testid anchors (`navigation.spec.ts`)
- [x] api-navigation — programmatic `window._swup.navigate()` API (`api-navigation.spec.ts`)
- [x] link-resolution — relative/absolute/external links, base URL, same-page links, resolveUrl option (`link-resolution.spec.ts`)
- [x] link-selector — SVG links, imagemap area links, custom linkSelector option (`link-selector.spec.ts`)
- [x] nested pages — `/nested/nested-1.html` + `/nested/nested-2.html` with `<base href>`, relative link resolution (`link-resolution.spec.ts`)

## Animation
- [x] animation-duration — 400ms CSS transition, correct out/in/total timing (`animation-timing.spec.ts`)
- [x] animation-complex — 600ms multi-property transition timing (`animation-timing.spec.ts`)
- [x] animation-keyframes — 700ms CSS keyframe animation timing (`animation-timing.spec.ts`)
- [x] animation-none — `transition: none` → instant navigation, hooks still fire, classes cleaned up (`animation-extra.spec.ts`)
- [x] animation-partial — only `#swup` container has transition, `aside` has none; 400ms timing from animated container (`animation-extra.spec.ts`)
- [x] animation-classes — is-changing/is-animating/is-leaving/is-rendering class lifecycle (`animation-classes.spec.ts`)
- [x] native-mode — View Transitions API, swup-native class, awaits transitions (`native-mode.spec.ts`)

## Page Lifecycle
- [x] markup — swup-enabled class added/removed, animation class sequence on html and container elements (`markup.spec.ts`)
- [x] events — custom DOM events (swup:*), swup:any wildcard, event bubbling, preventDefault (`events.spec.ts`)
- [x] page-load — page:load hook replacement and custom handlers (`page-load.spec.ts`)
- [x] visit-object — visit.from/to URLs, visit.to.html/document, trigger el/event, animation.name/wait/animate/native, meta, popstate (`visit-object.spec.ts`)

## Instance
- [x] instance — minimal Swup init on empty page, swup-enabled class, API, destroy, disable hook, default options, empty cache (`instance.spec.ts`)

## Caching
- [x] cache — pages cached/not cached, disable via options/navigation/visit object, marks from page:load, no POST cache (`cache.spec.ts`)

## History
- [x] history — pushState, replaceState via data-attr/API, popstate back/forward, direction, error handling (`history.spec.ts`)

## Scrolling
- [x] scrolling — anchor scroll, scroll to top, anchor-by-id/name, encoded/special chars, cross-page anchor, hash manipulation (`scrolling.spec.ts`)

## Special Visit Handling
- [x] ignore-visit — data-no-swup element/parent, ignoreVisit callback, custom path matcher (`ignore-visit.spec.ts`)
- [x] containers — multiple containers, custom via visit object, reload on mismatch (`containers.spec.ts`)
- [x] persisting — data-swup-persist elements kept across navigations (`persisting.spec.ts`)
- [x] redirects — server redirects followed, redirect target not cached (`redirects.spec.ts`)
- [x] request — Referer/X-Requested-With headers, 500 error, network error, fetch timeout (`request.spec.ts`)

## Integrations
- [x] alpinejs — Alpine.js swup:link:click + swup:any events in Alpine components (`alpinejs.spec.ts`)
- [x] plugins/body-class-plugin — body class updated on navigation (`plugins/body-class-plugin.spec.ts`)
- [x] plugins/scroll-plugin — scroll to anchor/top, cross-page anchor, hash manipulation (`plugins/scroll-plugin.spec.ts`)
