---
title: Alloy Project Plan
subtitle: 
layout: layouts/base.njk
---

## Project Setup

### Environment Setup

- Update FE development process to use Webpack, Babel and Polyfills (ECMAScript6/AngularJS/Angular/Vue).
- For now - single CSS bundle and single JS bundle. In grand scheme of things, we produce fairly small bundles on average:

|Project  |CSS  |CSS (gzip)  |JS  |JS (gzip)  |
|---------|---------|---------|---------|---------|
|ncc      | 136     | 28      | 240     | 106     |
|xcd      | 98      | 18      | 272     | 118     |
|gg       | 165     | 25      | 2100    | 379     |

- FE to discuss/extend/give BE a functional spec for a module. Help prevent missing features that are difficult to get into a module after the fact. eg, title attribute on an iframe (needs to be in Umbraco with explainer text, not constructed from a module name)

## Work to be Sprinted

- Article listing
  - default (news) card
  - featured (news) card
- Article (news) page
- Modules Layout List
  - layout for page modules (outer 'stripes')
  - layout for inner page modules
- Banners
- Navigation elements
  - sub items, expansion and animation
  - mobile shrunken state and animation
- Navigation layout
  - logo, nav, search
- Form elements (using Editor Templates)
  - checkbox
  - radio
  - input
  - select
- Form layout
  - inline
  - rows
- Search results
- Pagination
- Sitemap
- Breadcrumbs
- Cookie preferences
- Newsletter Signup
- Enquiry Form
- Social sharing widget

### Future Environment Setup

Have CSS and JS modules linked to pages/views (maybe RequireJS, or combo with Webpack chunks?)
Using Babel and Polyfills - deliver 'optimised' JS and polyfilled/old JS to 'supported' browsers, no-js to rest.
Agnostic JS dev - Vanilla/ECMAscript 6, AngularJS, Angular, Vue
Modular approach (Would be nice to get basic Alloy modules linked to their JS modules that make them function). Not always worked in the past, as design called for too different functionality/design, or module didn't have that spec, difficult to put those changes back into Alloy.
Additional custom/bespoke JS and modules - led by Design/UX/budget
