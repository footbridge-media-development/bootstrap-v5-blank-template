# Blank Bootstrap v5 Website Template
A blank Bootstrap v5 (using source SCSS) website template ready to be built. Blank with no dependencies.

## Customizing & Theming
To override a Bootrap v5 theme color, you must redefine the variable used in that theme. For example, overriding the primary theme color would be done like shown below:
```scss
$primary: #000000;
@import "..bootstrap/bootstrap";
```

However, adding an entirely new theme color would be done by merging a map with the existing theme colors map after importing bootstrap. Shown below:

```scss
$new-theme-colors: (
	some-name:#0000,
);

@import "..bootstrap/bootstrap";
$theme-colors: map-merge($theme-colors, $new-theme-colors);
```
