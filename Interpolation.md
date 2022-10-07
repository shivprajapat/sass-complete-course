# SASS Interpolation

Interpolation can be used almost anywhere in a Sass stylesheet to embed the result of a SassScript expression into a chunk of CSS. Just wrap an expression in #{} in any of the following places:

## use the Interpolation

### Margin

```
@mixin margin($position, $unit) {
    margin-#{$position}: $unit;
}

```
### Padding

```
@mixin padding($position, $unit) {
    padding-#{$position}: $unit + px;
}
```
```
// use interpolation margin

@include margin(left, 20px); // margin-left: 20px;
@include margin(right, 20px);
@include margin(top, 20px);
@include margin(bottom, 20px);

// use interpolation padding

@include padding(left, 20); // padding-left: 20px;
@include padding(right, 20);
@include padding(top, 20);
@include padding(bottom, 20);
```
