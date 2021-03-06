## ExtendedGCD

```
ExtendedGCD(n1, n2, ...)
```

> computes the extended greatest common divisor of the given integers. 

### Examples

``` 
>> ExtendedGCD(10, 15)
{5,{-1,1}}
``` 

`ExtendedGCD` works with any number of arguments:
``` 
>> ExtendedGCD(10, 15, 7)
{1,{-3,3,-2}}
``` 

Compute the greatest common divisor and check the result:
``` 
>> numbers = {10, 20, 14};

>> {gcd, factors} = ExtendedGCD(Sequence @@ numbers)
{2,{3,0,-2}}

>> Plus @@ (numbers * factors)
2
``` 

