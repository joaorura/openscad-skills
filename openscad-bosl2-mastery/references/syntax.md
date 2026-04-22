# BOSL2 Syntax Reference

## Common Modules
- **`cuboid([w, d, h], anchor=anchor, spin=spin, orient=orient, rounding=rounding, edges=edges)`**
- **`cyl(h=h, d=d, anchor=anchor, spin=spin, orient=orient, rounding=rounding)`**
- **`tube(h=h, id=id, od=od, anchor=anchor, spin=spin, orient=orient)`**
- **`rect([w, d], rounding=rounding, anchor=anchor)`** (2D)

## Anchor Names
- `CENTER`, `TOP`, `BOTTOM`, `LEFT`, `RIGHT`, `FRONT`, `BACK`
- `TOP+LEFT`, `BOTTOM+FRONT`, etc. (Compound anchors)

## Transformations
- `up(z)`, `down(z)`, `left(x)`, `right(x)`, `fwd(y)`, `back(y)`
- `move([x, y, z])`
- `xrot(a)`, `yrot(a)`, `zrot(a)`
- `rot([ax, ay, az])`
- `xflip()`, `yflip()`, `zflip()`
