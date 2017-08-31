# Parse String method examples

This is a collection of String parsing methods that I have needed in development.

_Example 1_: Parse string where the values are separated by ';' This is common when looking a property where the values are selected by a picklist.

```apex
@TestVisible
private Set<string> parseString(String selectedValues)
{
  Set<string> parsedSet = new Set<string>();

  if(String.isNotBlank(selectedValues))
  {
    List<string> values = selectedValues.split(';');
    parsedSet.addAll(values);
  }

  return parsedSet;
}
```
