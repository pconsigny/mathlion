<!-- Note: This file is automatically generated from source code comments. Changes made in this file will be overridden. -->

# Function isPositive

Test whether a value is positive: larger than zero.
The function supports types `number`, `BigNumber`, `Fraction`, and `Unit`.

The function is evaluated element-wise in case of Array or Matrix input.


## Syntax

```js
isPositive(x)
```

### Parameters

Parameter | Type | Description
--------- | ---- | -----------
`x` | number &#124; BigNumber &#124; Fraction &#124; Unit &#124; Array &#124; Matrix | Value to be tested

### Returns

Type | Description
---- | -----------
boolean | Returns true when `x` is larger than zero. Throws an error in case of an unknown data type.


## Examples

```js
isPositive(3);                     // returns true
isPositive(-2);                    // returns false
isPositive(0);                     // returns false
isPositive(-0);                    // returns false
isPositive(0.5);                   // returns true
isPositive(bignumber(2));     // returns true
isPositive(fraction(-2, 5));  // returns false
isPositive(fraction(1,3));    // returns false
isPositive('2');                   // returns true
isPositive([2, 0, -3]');           // returns [true, false, false]
```


## See also

[isNumeric](isNumeric.md),
[isZero](isZero.md),
[isNegative](isNegative.md),
[isInteger](isInteger.md)