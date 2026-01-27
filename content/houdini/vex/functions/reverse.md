---
breadcrumbs: Houdini 21.0 > VEX > VEX Functions
source: https://www.sidefx.com/docs/houdini/vex/functions/reverse.html
---

# reverse VEX function

> Returns an array or string in reverse order.

`string  reverse(string str)`

Returns a UTF-8 encoded string with the reversed *characters* (not bytes) from `str`. This is different from what `str[::-1]` returns.

`<type>[] reverse(<type>values[])`

Returns a reversed copy of the given array.

## Examples

```vex
reverse("hello") == "olleh";
reverse({1,2,3,4}) == {4, 3, 2, 1};
```