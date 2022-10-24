# My Resources - feel free to use

## Responsive Mixins sass/abstracts/\_responsive.scss

Mixins for:

- inline css Clamp
- css clamp insertions - also see my clamp tool https://clampy.leonlonsdale.co.uk
- media queries.

### Media query use:

Defaults to Min for mobile first

```scss
@include breakpoint(md) {
}
```

Or make it max for desktop first

```scss
@include breakpoint(md, max) {
}
```

or just put your own viewport values in:

```scss
@include breakpoint(965, max) {
}
```

### Clamps

```scss
@include getClamp(font-size, minFontSize, maxFontSize, minViewport, maxViewport) @include getClamp(
    padding,
    minPadding,
    maxPadding,
    minViewport,
    maxViewport
  );
```

or

```scss
#{insertClamp(minSize, maxSize, minViewport, maxViewport)}
```

Can also use the breakpoints:

```scss
@include getClamp(font-size, minFontSize, maxFontSize, sm, xl) #{insertClamp(
    minSize,
    maxSize,
    sm,
    xl
  )};
```

## Colors.scss

This is the Tailwind colour palette put into Scss variables. Please see their page: https://tailwindcss.com/docs/customizing-colors

## Sprite.svg

Again, tailwind stuff - this is a sprite of their free Heroicons. Please isit their page https://heroicons.com/
