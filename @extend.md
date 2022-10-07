# @extend

## Create a extend

```
%btn{
    font-size: 15px;
    font-weight: 900;
    text-transform: uppercase;
    padding: 10px 32px;
    border-radius: 5px;
    border: 1px solid #ddd;
}
```

## use this @extend 

```
.btnred {
   color: red;
   @extend %btn;
}
.btngreen {
   color: green;
   @extend %btn;
}
```


## html code


```
<div>
    <button class="btnred">Extend</button>
    <button class="btngreen">Extend</button>
</div>
```