---
breadcrumbs: Houdini 21.0 > VEX > VEX Functions
source: https://www.sidefx.com/docs/houdini/vex/functions/attribclass.html
---

# attribclass VEX function

> Returns the class of a geometry attribute.

`string  attribclass(<geometry>geometry, string attribute_name)`

Show/hide arguments 

`<geometry>`

When running in the context of a node (such as a wrangle SOP), this argument can be an integer representing the input number (starting at 0) to read the geometry from.

Alternatively, the argument can be a string specifying a geometry file (for example, a `.bgeo`) to read from. When running inside Houdini, this can be an `op:/path/to/sop` reference.

`attribute_name`

The name of the attribute to read.

If attributes with the same name exist at multiple “levels”, returns the *lowest level* at which the attribute exists. For example, if there is a primitive attribute `foo` and a vertex attribute `foo`, `attribclass(0, "foo")` will return `"vertex"`.

Returns

A string describing the class (`"detail"`, `"prim"`, `"point"`, or `"vertex"`) of the given attribute. If the attribute does not exist, returns an empty string (`""`).