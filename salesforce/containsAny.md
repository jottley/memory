# Compare two sets to see if there is at least one value that matches

_Example 1_: Sets are of string values

```apex
@TestVisible
private boolean containsAny(Set<String> a, Set<String> b)
{
  if (a != null && b != null)
  {
      for (String value : a)
      {
          if (b.contains(value))
          {
              return true;
          }
      }
  }

  return false;
}
```
