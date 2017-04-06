# CSS/SCSS Guidelines

## Introduction
This document captures my current (unstructured) thoughts on styling. It is a living document and always changing and flexing to fit project/team or as they pop into my head. 

## Guiding Principle
* Clarity > Efficiency > Consistency > Beauty

## IDE/Editor Setup
* 4 space indents, not tabs
* 80-character maximum lines
* Multiline declarations
* Use .editorconfig for teams

## General Ideas
* Use classes predominately to lower specificity and complexity
* Abbreviate class names only if necessary and avoid short hand when possible. A good class name should be easily searchable and readable. (Complexity is harder to modify, maintain, reuse, etc.) 
* Each declaration has a line break. Multiple declarations on a single line is harder to read and make file diffs more challenging.

## Block Spacing
* Single line break between closely related blocks
* Two line breaks between somewhat related blocks
* Unrelated blocks should be separate partials

## Commenting
* Major Comments Style - Block
* Minor Comments Style - Inline/Above statement

## CSS Terminology
* selector (ex. body, .nav)
* property (ex. padding)
* value (ex. 2rem)
* declaration or rule (property/value pair) (ex. font-size: 1.5rem) 
* rule set / block: a selector and one or more declarations within curly braces

## Naming Convention (BEM-like)
* Block__Element--Modifier

## Namespace/Prefix Classes (Be obvious, not clever.)
* JS hooks (ex. js-) - There signify JS, not style, hooks 
* utilities (ex. u- or util-): Should serve a single purpose and be immutable (never changing) (ex. .u-margin-none)
* state (ex. is-, has-): represents state of element and always used with another selector (ex. .panel.is-active)

## Scoping sections for WYSIWIG content/third-parties
* Wrapping classes for environments that use other frameworks or legacy content

## Styling elements
* Don't create .h1, .h2, etc exclusively (Decouple semantics from styles, use descriptives: ex. '--small')
* Be verbose
* Bottom margins for component spacing

## Spacing Utility Classes
* Padding (ex. .u-padding--small)
* Margin (ex. .u-margin--large)

## Sass Conventions
* Project Table of Contents (index.scss)
* Declaration/Feature Ordering (@include)
* Multi folder/file organization
* Common helpers (Mixins for media queries, spacing, etc)
* Single location for variables
* Media queries with component it affects (using Sass nesting)
* Minimize nesting as much as possible
* Keep it simple

## References
* Harry Roberts - [CSS Guidelines](http://cssguidelin.es), [CSS Wizardry](https://csswizardry.com/)
* [SMACSS](https://smacss.com/) by [Jonathan Snook](https://snook.ca/) 
* [Sass Guidelines](https://sass-guidelin.es/)
* [Lightning Design System](https://lightningdesignsystem.com/)
* [The Salesforce Team Model for Scaling a Design System](https://medium.com/salesforce-ux/the-salesforce-team-model-for-scaling-a-design-system-d89c2a2d404b) by Jina Bolton
* [Many Nathan Curtis Medium articles](https://medium.com/@nathanacurtis)
* [Battling BEM (Extended Edition)](https://www.smashingmagazine.com/2016/06/battling-bem-extended-edition-common-problems-and-how-to-avoid-them/) by David Berner @daveordead
* [@mdo Code Style](http://codeguide.co) by Mark Otto
