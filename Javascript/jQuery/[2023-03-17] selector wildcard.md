# jQuery Selector with Wildcard

Sumber: <https://stackoverflow.com/questions/190253/jquery-selector-regular-expressions>

- If you're finding by **Contains** then it'll be like this

```javascript
$("input[id*='DiscountType']").each(function (i, el) {
    //It'll be an array of elements
});
```

- If you're finding by **Starts With** then it'll be like this

```javascript
$("input[id^='DiscountType']").each(function (i, el) {
    //It'll be an array of elements
});
```

- If you're finding by **Ends With** then it'll be like this

```javascript
$("input[id$='DiscountType']").each(function (i, el) {
    //It'll be an array of elements
});
```

- If you want to select elements which **id is not a given string**

```javascript
$("input[id!='DiscountType']").each(function (i, el) {
    //It'll be an array of elements
});
```

- If you want to select elements which **name contains a given word, delimited by spaces**

```javascript
$("input[name~='DiscountType']").each(function (i, el) {
    //It'll be an array of elements
});
```

- If you want to select elements which **id is equal to a given string or starting with that string followed by a hyphen**

```javascript
$("input[id|='DiscountType']").each(function (i, el) {
    //It'll be an array of elements
});
```
