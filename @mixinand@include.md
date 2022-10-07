# Sass @mixin and @include

## Dynamically CSS for position-absolute

```
@mixin position-absolute($top: null, $left: null, $right: null, $bottom: null) {
    position: absolute;
    top: $top;
    left: $left;
    right: $right;
    bottom: $bottom;
}
```
## Dynamically CSS for background image

```
@mixin bgImage($image) {
    background: url($image);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    background-blend-mode: overlay;
}
```
### include

```
@include bgImage("/images/1.jpg");
```

## FlexBox 

```
@mixin flexCenter {
    display: flex;
    align-items: center;
    justify-content: center;
}
```
```
@mixin flexSpace {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```
```
@mixin flexVertical {
    display: flex;
    align-items: center;
}
```
### include

```
@include flexCenter;
@include flexSpace;
@include flexVertical;

## Main Heading

```
@mixin heading {
    color: $primary;
    font-size: $heading + 4 + px; // 30px
}
```
