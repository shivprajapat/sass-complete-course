# Sass Selector Functions

The selector functions allow you to manipulate the CSS selectors in a stylesheet. All of the functions except selector-nest(), selector-append() prohibit the use of the parent selector &.

### selector-nest,

```
$selector-n: selector-nest('.home','&_heading');
// $selector-n: selector-nest('.home','&_heading',' &:hover');
// $selector-n: selector-nest('header','h1');
```
### selector-append,

```
$selector-a: selector-append('.home','.active');
```
### use 

```
#{$selector-n} {background-color: red;}
```
### use,
```
#{$selector-a} {background-color: red;}
```