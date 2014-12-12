sass-style-guide
================

Sass style guide

Shared conventions for the use, understanding and creation of variables:

## Table of contents

1. Conventions
2. Nomenclature
3. Variables order
4. Variables names
5. Properties

### Conventions

Use lower case to set colors.

/* DON'T */

\#F0F0F0;


/* DO */

\#f0f0f0;

When possible, use the shorthand sintaxis.

/* DON'T */

\#CCCCCC;


/* DO */

\#ccc;

Opacity property setup:

/* DON'T */

rgba(255, 255, 255, 0.5)


/* DO */

rgba(255, 255, 255, .5)

### Nomenclature

${element}-{property.name}

E.g.:

$bubble-text-color;
$legend-margin;
$icon-opacity;

### Variables order

Order: ${component}-{variant}-{type}-{state}-property-name}

1. component (e.g.: input, bubble, tooltip).
2. variant (e.g.: btn-primary, btn-secondary, box-list-item).
3. type (e.g.: read-only)
4. state (e.g.: focus, hover, disabled).
5. ie (only to indicate IE).
6. property-name (e.g.: bg-color, border, padding).

E.g.:

$input-read-only-hover-bg-color;
$btn-primary-active-padding;

*Variable name must be conceptual, not necessarily referred to css element.*

/* DON'T */
$pagination-li;

/* DO */
$pagination-current-page;

### From css propertyes to variable names

Color: ${element}-text-color;

Font-size: ${element}-text-size;

Vertical-align: ${element}-v-align;
