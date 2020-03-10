---
title: Alloy Project Plan
subtitle: 
layout: layouts/base.njk
---

## Project Setup

- Update FE development process to use Webpack, Babel and Polyfills (ECMAScript6/AngularJS/Angular/Vue).
- For now - single CSS bundle and single JS bundle. In grand scheme of things, we produce fairly small bundles on average:

|Project  |CSS      |CSS (gzip) |JS       |JS (gzip) |
|---------|---------|-----------|---------|----------|
|ncc      | 136     | 28        | 240     | 106      |
|xcd      | 98      | 18        | 272     | 118      |
|gg       | 165     | 25        | 2100    | 379      |

- Suggestion that FE to discuss/extend/give BE a functional spec for a module.

  Helps prevent missing features that are difficult to get into a module after the fact. eg, title attribute on an iframe (needs to be in Umbraco with explainer text, not constructed from a module name)

## Future Setup

- Modular CSS and JS - Have CSS and JS modules linked to pages/views (maybe RequireJS, or combo with Webpack chunks?)
- Modular approach (Would be nice to get basic Alloy modules linked to their JS modules that make them function). Not always worked in the past, as design called for too different functionality/design, or module didn't have that spec, difficult to put those changes back into Alloy.
- Using Babel and Polyfills - deliver 'optimised' JS and polyfilled/old JS to 'supported' browsers, no-js to rest. Separate support of older browsers/older technology.
- Agnostic JS dev - Vanilla/ECMAscript 6, AngularJS, Angular, Vue
- Additional custom/bespoke JS and modules - led by Design/UX/budget
