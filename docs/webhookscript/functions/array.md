### array_contains(***array*** array, ***string/number*** needle) : bool

Returns true or false depending on whether ***array*** contains a value equal to ***needle***.

To check whether a key exists, use the `array_has` function.

```javascript
employees = [6547: 'Simon', 235345: 'Jack', 4657: 'Jim']

dd(array_contains(employees, 'Simon'))
// -> true
```

### array_copy(***array*** array) : array

Returns a copy of ***array***

### array_diff(***array*** array1, ***array*** array2) : array

Returns the items of array1 that are not present in array2 while keeping the array indices.

### array_get(***array*** array, ***string/number*** index, ***any*** default) : any

### array_has(***array*** array, ***string/number*** key) : bool

Returns true if `array` contains `key`, and false if it does not.

To check whether a value exists, use the `array_contains` function.

```javascript
employees = [6547: 'Simon', 235345: 'Jack', 4657: 'Jim']

dd(array_has(employees, 235345))
// -> true
```

### array_join(***array*** array, ***string*** joiner) : string

Returns a string where all the values are joined by `joiner`.

```javascript
['hello', 'world'].join(',')
-> "hello,world"
```

### array_keys(***array*** array) : array

Returns the keys of an array.

### array_length(***array*** array) : number

### array_map(***array*** array, ***func*** function)

Runs function with each array value, and returns array with key as result.

```javascript
employees = ['Simon', 'Jack', 'Jim']

result = array_map(employees, function (employee) {
    return 'Hello, '+employee+'!'
})

dd(result)

// -> [0: "Hello, Simon!", 1: "Hello, Jack!", 2: "Hello, Jim!"]
```

### array_number_of(***array***, ***string/number*** value) : number

Returns amount of ***value***

### array_pop(***array*** array) : any

Pop element off end of array

### array_push(***array*** array, ***any*** value) : any

Adds ***value*** to end of ***array*** and returns ***value***

### array_random(***array*** array) : any

Returns random value of ***array*** 

### array_reverse(***array*** array) : array

Returns ***array*** in reverse order

```javascript
employees = [6547: 'Simon', 235345: 'Jack', 4657: 'Jim']

dd(array_reverse(employees))
// -> [0: "Jim", 1: "Jack", 2: "Simon"]
```

### array_shuffle(***array*** array) : array

Returns shuffled version of ***array***

### array_sort(***array*** array) : array

Sorts ***array*** by its values. Keys are kept as-is.

### array_values(***array*** array) : array

Returns the values of an array.

```javascript
employees = [6547: 'Simon', 235345: 'Jack', 4657: 'Jim']

dd(array_values(employees))

// -> [0: "Simon", 1: "Jack", 2: "Jim"]
```

### to_array(***array*** array) : array

Returns ***array***.