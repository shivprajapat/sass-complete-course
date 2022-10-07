# SASS @function

Functions allow you to define complex operations on SassScript values that you can re-use throughout your stylesheet. They make it easy to abstract out common formulas and behaviors in a readable way.


## Half the section size

```
$container: 1200;

@function half($width) {
    @return $width/2 + px;
}

@function col($width) {
    @return $width/4 + px;
}

@function flex($x, $y) {
    @return $x/$y;
}

```

### use the code

```
.divs {
    width: half($container);
    div {
        width: col($container);
        height: col($container);
        background-color: red;
    }
}

```
```
.flexs {width: (300 / 3 + px);}
```
### Dynamic Font Size for 1em to 16px

```
@function em($value, $base: 16) {
    @return #{$value / $base}em;
}
```

### Example Dynamic font size 

```
p {font-size: em(16);}
```
### Dynamic Font Size for 16px to 1em

```
$base-font-size: 16px;
@function em($px, $base: $base-font-size) {
    @return ($px / $base) * 1em;
}
```

### Example Dynamic font size 

```
h1 {font-size: em(16px, 16px);}
```