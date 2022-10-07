# @at-root

```
@media section {
    .container {
        .item {
            background-color: red;
}
        @at-root {
            .item {
                background-color: red;
            }
        }
    }
}
```

## sass to the compiler css 

```
@media section {
  .container .item {
    background-color: red;
  }
  .item {
    background-color: red;
  }
}
```