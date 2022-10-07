# Sass Variables

Variables are a way to store information that you can re-use later.

With Sass, you can store information in variables, like:

strings
number
colors
map
nulls

## strings


```
$default-font: 'Lucida';

font-family: $default-font, "Ariel", sans-serif;
```

## number

For example, the following operations are valid:

```
$main-heading: 25;

font-size: $heading + 10 + px; // 30px
```

## colors

```
$primary: #d9354c;

background-color: $primary;
```

## map 

```
$red-map: (light: #e57373, medium: rgb(29, 9, 9), black: #000);

background-color: map-get($red-map, light);

background-color: map-get($red-map, medium);

background-color: map-get($red-map, black);
```

## nulls

```
@mixin position-absolute($top: null, $left: null, $right: null, $bottom: null) {
    position: absolute;
    top: $top;
    left: $left;
    right: $right;
    bottom: $bottom;
}

@include position-absolute($top: 0, $left: 0);
```

