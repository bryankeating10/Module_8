# **:wrench: Repository Edits**
*Bryan Keating*

## Dockerhub URL
https://hub.docker.com/bryankeating10/Module8

## App
Added power function:
```
def power(a: Number, b: Number) -> Number:
    # Dockstring
    
    result = a ** b
    return result
```

## Testing
Added testing for power function:
```
@pytest.mark.parametrize(
    "a, b, expected",
    [
        (2,3,8),           # Test raising a positive integer to a positive integer power
   ...
   ],
    ids=[
        "power_positive_integer_to_positive_integer",
   ...
    ]
)
def test_power:
   # Docstring

   result = power(a, b)
   assert result == expected, f"Expected power({a}, {b}) to be {expected}, but got {result}"

```