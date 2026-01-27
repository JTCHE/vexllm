---
breadcrumbs: Houdini 21.0 > VEX > VEX Functions
source: https://www.sidefx.com/docs/houdini/vex/functions/hasprimattrib.html
---

# hasprimattrib VEX function

> Returns if a geometry prim attribute exists.

`int  hasprimattrib(<geometry>geometry, string attribute_name)`

Show/hide arguments 

`<geometry>`

When running in the context of a node (such as a wrangle SOP), this argument can be an integer representing the input number (starting at 0) to read the geometry from.

Alternatively, the argument can be a string specifying a geometry file (for example, a `.bgeo`) to read from. When running inside Houdini, this can be an `op:/path/to/sop` reference.

Returns `1` if the attribute exists, or `0` otherwise.

## Examples

```vex
// Determine if the P attribute exists.
int exists = hasprimattrib("defgeo.bgeo", "P");
```