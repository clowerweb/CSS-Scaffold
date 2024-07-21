# iSynergy CSS Scaffolding library

## Introduction

This library serves as a base that can be used for any new projects.
It provides useful rules for resetting browser defaults on various elements,
a way to set variables for colors, sizes, etc., and classes for display modes,
margins, padding, alignments, colors, etc.

## Setting variables

All the variables are defined in the `:root` directive and should be pretty straightforward.
Note that `--desktop-font-size`, `--tablet-font-size`, and `--mobile-font-size` MUST be
defined in `px` units and not `rem`, `em`, `pt`, or `%` units. Also, as a general rule, 
anything that is 1px should be defined in `px` units as well so that they don't get smaller
than 1px on tablet/mobile.

Feel free to add your own new variables as needed!

## Defaults

The defaults are all under the `body, html`, `headings`, `form element`, and `links/buttons` sections
(where elements are used as selectors instead of classes). Change these as needed (for the most part,
you probably won't need to after you've set the variables).

## Classes

### Class naming conventions

- `.b-*` - Border - Adds a border to the element. Example: `bl-secondary` adds a left border in the
secondary color.
- `.m-*` - Margin - Adds a margin to the element. Example: `mt-5` adds a 5px margin to the top of the
element.
- `.p-*` - Padding - Adds padding to the element. Example: `pb-5` adds 5px of padding to the bottom of
the element.
- `.w-*` - Width - Adds a width to the element. Example: `w-30` adds a width of 30% to the element.
- `.max-w-*` - Max width - Adds a max width to the element. Example: `max-w-20` adds a max width of 20%
to the element.
- `.min-w-*` - Min width - Adds a min width to the element. Example: `min-w-60` adds a min width of 60%
    to the element.
- `.display-*` - Display mode - Sets the display mode for the element (examples: `display-block`
or `display-flex`).
- `.align-*` - Flex align - Example: `align-baseline` adds `jalign-items: baseline` to the element.
- `.justify-*` - Flex justify - Example: `justify-center` adds `jusity-content: center` to the element.
- `.flex-*` - Flex grow/shrink/basis - Example: `flex-11a` adds `flex: 1 1 auto` to the element.
- `.color-*` - Sets the font color - Example: `color-primary` sets `color: var(--primary-color)` on the
element.

#### Targeting sides of an element

With some classes (such as border, margins, and padding), you can target one or more sides of an element
to apply the rule to.

- `.*t-*` - The top of the element. For example: `bt-primary` adds a `border-top` to the element in the
primary color. Other examples: `mt-10` adds a 10px `margin-top`, and `pt-10` adds 10px of `padding-top`.
- `.*r-*` - The right of the element. Example: `mr-10`.
- `.*b-*` - The bottom of the element. Example: `pb-10`.
- `.*l-*` - The left of the element. Example: `bl-secondary`.
- `.*x-*` - The left and right of the element. Example: `mx-auto` sets `margin-left` and `margin-right` to
`auto`.
- `.*y-*` - The top and bottom of the element. Example: `py-15` sets `padding-top` and `padding-bottom` to
`15px`.
- If there is no x/y/t/r/b/l in the class, it will apply to all 4 sides. Example: `m-20` will apply a 20px
`margin` to the top, right, bottom, and left of the element.

### Links & Buttons

Defined in the `links/buttons` section.

- `.underline` - Underlines text.
- `.avia-button` - Rules for buttons added via the content builder.
- `.no-hover .avia-button` - Changes the hover behavior for sections that have the `no-hover` class.
- `.has-arrow` - sample class that adds an arrow icon to the right size of a link or button.

### Borders

Defined in the `borders` section.

- `.b-primary` - Adds a border with the width `--bw-lg` and color `--primary-color` to the element
(all the way around).
- `.br-secondary` - Adds a border with the width `--bw-lg` and color `--primary-color` to the right
side of the element.
- All the other x/y/t/r/b/l rules apply here as well (see "Targeting sides of an element").

### Margins

Defined in the `margins` section.

- `.m-20` - Adds a margin of 20px to all sides of the element.
- All the other x/y/t/r/b/l rules apply here as well (see "Targeting sides of an element").

### Padding

Defined in the `padding` section.

- `.p-20` - Adds 20px of padding to all sides of the element.
- All the other x/y/t/r/b/l rules apply here as well (see "Targeting sides of an element").

### Misc utilities

- `.flex-row` - Sets `flex-direction` to `row`.
- `.flex-col` - Sets `flex-direction` to `column`.
- `.flex-row-reverse` - Sets `flex-direction` to `row-reverse`.
- `.flex-col-reverse` - Sets `flex-direction` to `column-reverse`.
- `.flex-wrap` - Sets `flex-wrap` to `wrap`.
- `.underline` - Underlines text.
- `.uppercase` - Uppercases text.
- `.no-hover` - Use on a parent container if you don't want a certain button to have a hover effect.
- `.has-arrow` - Adds an arrow icon to the right size of a link or button.
- `.italic` - Makes text italic.
- `.font-lighter` - The lightest font weight (defined under the `--font-weight-lighter` variable).
- `.font-light` - The light font weight (defined under the `--font-weight-light` variable).
- `.font-normal` - The normal font weight (defined under the `--font-weight-normal` variable).
- `.font-bold` - The bold font weight (defined under the `--font-weight-bold` variable).
- `.font-bolder` - The boldest font weight (defined under the `--font-weight-bolder` variable).
- `.dark` - Defines text colors for sections with dark backgrounds.
- `.sr-only` - For hiding an element (but keeping it visible to screen readers).
