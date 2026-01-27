---
breadcrumbs: Houdini 21.0 > VEX > VEX Functions
source: https://www.sidefx.com/docs/houdini/vex/functions/insert.html
---

# insert VEX function

> Inserts an item, array, or string into an array or string.

`void  insert(string &str, int index, string value)`

Inserts the `value` into the string `str` at the given `index`.

If `index` is greater than the length of the string, the `value` will simply be appended to the existing `str`.

`void  insert(<type>&array[], int index, <type>value)`

`void  insert(<type>&array[], int index, <type>values[])`

Inserts the items or items into the `array` starting at the given `index`.

If `index` is greater than the length current length of the `array`, the function will fill the gaps with uninitialized values (for example, `0` or the empty string).

-   If the `index` is negative, it counts from the *end* of the string or array you're inserting into. (If the negative number is greater than the string/array length, it is clamped to `0`.)
    
    For example, to insert the number `100` as the second-to-last item in an array:
    
    ```vex
    insert(numbers; -1; 100)
    ```
    

`int  insert(dict &dstdict, string dstkey, dict srcdict, string srckey)`

Copies the value from `srcdict[srckey]` into `dstdict[dstkey]`. This will preserve the underlying type of the value. If the key is not in the source dictionary, it will be removed from the destination dictionary. The result is `1` if the key existed in the destination dictionary before the update, and `0` if it did not.

`void  insert(dict &dstdict, dict srcdict)`

Merges `srcdict` into `dstdict`. Keys that match will be overwritten by values in the source dictionary.