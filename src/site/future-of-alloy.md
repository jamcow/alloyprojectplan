---
title: . . . 
subtitle: 
layout: layouts/base.njk
---

![](/images/bttf.jpg)

## Future of Alloy

- Is Alloy living up to expectations?
- What would we like from Alloy going forwards?
- Should we use LESS / Sass / Other?
- Should we use BEM / Utilities / Other (Tailwind)?
- When should we use CSS Grid / Flex / Other (and when shouldn't we)?
- Should we use Gulp / Webpack / Other?

## Notes: from meeting [2020-03-10]

Alloy's not living up to expectations. But it didn't really set any to start with other than to compile CSS and static site.

Majority of CSS modules are started from scratch for new projects, little to no re-use nor fed back into base Alloy project.

- Strip back legacy crud, with cleaner setup.
- Use SassDocs or similar to document existing Mixins and Planifolia.
- Replace Normalize with modern standards.
- Redefine Objects and Components to Layouts and Components.
- Modularise CSS.
- New mixins for spacing (margins and paddings).
- Make variables file more intuitive and inline with style guide.
- Use CSS Variables more (legacy browsers will get a more basic look and feel, where PostCSS can't flatten the variable fallbacks)

Continue using Sass

Continue with BEM and some additional utility classes. Perhaps using utility classes for layout (more dynamic layouts based on Razor logic and content). Tom to re-make an existing BEM card with Tailwinds.css

Make some common layout patterns with both flex and grid (and floats) with fallbacks.

Ditch Gulp, use Webpack to compile CSS and JS, for now create single bundle, can work to later make it split bundle into chunks for different pages.

### More notes

- Migrate to Webpack, Babel and Polyfills.
- FE and BE to discuss modules before coding/implementation (getting/sharing data in modules and naming conventions).
- FE to make modules (CSS, HTML and JS per module folder) with aim for them to be reusable modules.
- May need functional CSS, and appearance CSS, or maybe we comment in the CSS what is functional and what's appearance, to help make it easier to strip down for new projects.
- Look to further separate layout and design.
- There will be issues with getting and populating model data for each module, and integrating plain HTML back to CSHTML files. Accessibility and easy-to-miss changes may be troublesome to keep in sync.
- Code reviews at each sprint - discuss implementation, coding standards and setup.
