# @content Directive

## create responsive mixin

```
@mixin media($width) {
    @media screen and (max-width: $width) {
        @content;
    }
}
```

## use responsive mixin

```
body {
    @include media(1200px) {
        background: red;
    }
    @include media(1024px) {
        background: blue;
    }
    @include media(768px) {
        background: green;
    }
    @include media(576px) {
        background: pink;
    }
}
```