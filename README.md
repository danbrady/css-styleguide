# CSS/SCSS Guidelines

## Introduction
This document captures my current thoughts on styling. It is a living document and always changing and flexing to fit project/team.

## Foundation
* Clarity > Efficiency > Consistency > Beauty

## IDE/Editor Setup
* 4 space indents, not tabs
* 80-character maximum lines
* Multiline declarations

## Indenting

## Alignment

## Line Breaks between sections

## Commenting
* Major Comments Style
* Minor Comments Style

## CSS Terminology
* selector
* property
* value
* declaration (property/value pair)

## Naming Convention (BEM-like)
* Block__Element--Modifier

## Namespace Classes
* JS hooks (js-)
* utilities (u-)
* state (is-, has-)

## Scoping sections for WYSIWIG content/third-parties
* Wrapping classes for environments that use other frameworks or legacy

## Styling elements
* Don't create .h1, .h2, etc (Decouple semantics from styles, use descriptives: ex. '--small')
* Be verbose
* Bottom margins for component spacing

## Spacing Classes

## Sass conventions
* Project Table of Contents (index.scss)
* Declaration/Feature Ordering (@include)
* Multi folder/file organization
* Common helpers (Mixins for media queries, spacing, etc)
* Single location for variables
* Media queries with component it affects (using Sass nesting)

## References
* Harry Roberts - [CSS Guidelines](http://cssguidelin.es)
* SMACSS
* Sass Guidelines
* Lightning Design System
* Jina Bolton article
* Nathan Curtis blog/slides
* @daveordead smashing magazine article
* @mdo Code Style - [@mdo Code Style](http://codeguide.co)
