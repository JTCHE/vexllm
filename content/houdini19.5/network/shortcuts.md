---
breadcrumbs: Houdini 19.5 > Networks and parameters
source: https://www.sidefx.com/docs/houdini19.5/network/shortcuts.html
---

# Network editor shortcuts

> A quick reference for hotkeys and user interface shortcuts in the network editor.

Tip

Look through the menus to discover network editor functionality and keyboard equivalents.

## View keys

[More info](https://undefined/docs/houdini19.5/network/navigate)

Key

Alternate

Description

Space + LMB

MMB

Pan

Space + RMB

mouse\_wheel

Zoom

H

Pan and zoom to show all nodes

G

Pan and zoom to show the selected nodes

## Adding to the network

[More info](https://undefined/docs/houdini19.5/network/nodes)

Key

Description

⇥ Tab

Add a node to the current network from a menu.

\=

Add a File node (if available in the current network).

⇧ Shift + O

Add a [network box](https://undefined/docs/houdini19.5/network/organize#netbox) to the current network. If any nodes are selected, they are added to the box.

⇧ Shift + P

Add a [sticky note](https://undefined/docs/houdini19.5/network/organize#notes) to the current network.

## Wiring

[More info](https://undefined/docs/houdini19.5/network/wire)

Key

Description

LMB on connector

Drag between two connectors, or click one connector and then the other, to wire nodes together.

RMB on connector

Insert a new node before any currently connected nodes.

MMB on connector

Branch a new node off the connector.

Alt + LMB on node

Show a menu of connectors to start wiring from. This can be useful when you're too zoomed out to hit the connectors.

Y

Hold Y and drag across wires to cut (disconnect) them.

Shake node

Disconnect from any wires.

Alt + LMB on wire

Add [dot](https://undefined/docs/houdini19.5/network/wire#dots).

You can also Alt\-click while drawing a wire to insert a dot “on the fly”.

Alt + LMB on dot

[Pin/unpin](https://undefined/docs/houdini19.5/network/wire#dots) the dot.

You can also ⌃ Ctrl + Alt\-click while drawing a wire to insert a pinned dot “on the fly”.

8 while dropping node

Holding 8 temporarily disables wiring the node in if you drop the node on a wire. This lets you drop a node without worrying about accidentally rewiring it if there is an existing wire in the same area.

If you've turned off **Tools ▸ Allow dropping nodes on wires**, then holding 8 temporarily *enables* dropping a node onto a wire to wire it in.

## Tools

Key

Description

P

Toggle a floating parameter editor pane in the top right corner of the network.

⇧ Shift + W

Toggle a tree view of the complete network hierarchy on the left of the network.

O

Toggle the [network overview](https://undefined/docs/houdini19.5/network/navigate#overview) in the bottom left corner of the network.

C

Toggle the [color palette](https://undefined/docs/houdini19.5/network/organize#custom) in the bottom right corner of the network.

Z

Toggle the [shape palette](https://undefined/docs/houdini19.5/network/organize#custom) in the bottom right corner of the network.

## Navigation

[More info](https://undefined/docs/houdini19.5/network/navigate)

Key

Alternate

Description

Double-click

Enter

Double-click a node to go inside, or select it and press Enter.

U

Press U to go up a level.

⌃ Ctrl + *N*

Press ⌃ Ctrl and a number from 1-5 to set a quick mark.

⇧ Shift + *N*

Press ⇧ Shift and a number from 1-5 to return a set quick mark.

\` (backtick)

Go back to the previous view. This lets you quickly switch back and forth between two views, possibly in different networks.

PgUp

Select the node upstream (connected to the input) of the currently selected node.

PgDn

Select the node downstream (connected to the output) of the currently selected node.

⇧ Shift + PgUp

Select the previous sibling node of the currently selected node.

⇧ Shift + PgDn

Select the next sibling node of the currently selected node.

## Working with nodes

[More info](https://undefined/docs/houdini19.5/network/nodes#info)

Key

Description

MMB

Press MMB on a node to show the [node info window](https://undefined/docs/houdini19.5/network/nodes#info) while you hold the button down. This is a quick way to glance at the information in the info window.

⇧ Shift + MMB

Press ⇧ Shift + MMB on a node to show the node info window without cooking the node. This may be useful for nodes that take a long time to cook.

Alt + drag node

Create a copy of the node.

S + drag box selection

Holding S locks the drag to be a selection. This can be useful if there’s not enough “empty” space to start a box selection without hitting something else.

## Laying out nodes

// Note: have to indent this so the Include below doesn’t get sucked under this heading.

[More info](https://undefined/docs/houdini19.5/network/layout)

Key

Description

Drag node + Space

When dragging a node, hold Space to lock the mouse pointer inside the network view. This lets you autoscroll long distances without worrying about the mouse pointer going outside the pane.

A

Hold A and drag up/left on a node to automatically lay out the upstream nodes. Drag down/right to lay out the downstream nodes. If some nodes are selected, only those nodes are moved.

⇧ Shift + A

Select the nodes to align, then hold ⇧ Shift + A and drag on the node to align to. Drag left/right to align horizontally, or up/down to align vertically.

Alt + A

Select the nodes to move, then hold Alt + A and drag left/right on a node. Drag left/right to distribute horizontally, or up/down to distribute vertically.

:include flags#keys:

## Clicks and drags

Action

Description

LMB

Select.

⇧ Shift + LMB

Add to selection.

⌃ Ctrl + LMB

Remove from selection.

Alt + LMB

Start wiring from a node.

Alt + ⇧ Shift + LMB

Select node and all its inputs.

Alt + ⌃ Ctrl + LMB

Select node and all its outputs.

Alt + ⇧ Shift + ⌃ Ctrl + LMB

Select node and all inputs and outputs.

Drag LMB

Move.

Drag ⇧ Shift + LMB

Move node and all its inputs.

Drag ⌃ Ctrl + LMB

Move node and all its outputs.

Drag Alt + LMB

Drag out a copy of selected node(s).

Drag Alt + ⇧ Shift + LMB

Drag out a copy of the selected node(s) and all inputs.

Drag Alt + ⌃ Ctrl + LMB

Drag out a copy of the selected node(s) and all outputs.

Drag Alt + ⌃ Ctrl + ⇧ Shift + LMB

Drag out a [reference copy](https://undefined/docs/houdini19.5/network/copying) of the selected node(s).

## Notes and network boxes

[More info](https://undefined/docs/houdini19.5/network/organize)

Key

Description

⇧ Shift + P

Add a sticky note.

⇧ Shift + O

Put selected items in a network box.

⇧ Shift + J

Minimize any selected notes and/or boxes.

⇧ Shift + K

De-minimize any selected notes and/or boxes.

⇧ Shift + M

Shrink the selected network box to fit its contents.

## Finding nodes

Key

Alternate

Description

⌃ Ctrl + F

/

Open the find dialog.

⌃ Ctrl + G

\>

Select next match in the last search results.

⇧ Shift + ⌃ Ctrl + G

<

Select previous match in the last search results.