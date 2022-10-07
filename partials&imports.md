# What is Partials in SASS

A partial is a Sass file named with a leading underscore. You might name it something like _partial.scss . The underscore lets Sass know that the file is only a partial file and that it should not be generated into a CSS file. Sass partials are used with the @use rule.


## => use the _partial.scss format 

## create file format

### _header.scss

### _home.scss

### _footer.scss


## use scss file for index.scss


## file Format


### @import: ;
### @use: ;

```
@import './footer.scss';
@import './header.scss';
```
```
@use  './home';
```