Vim Tips
=======

1. Disable mouse control if it's not already disabled by default:
    ```:set mouse=```
2. `C-x C-f` for filename completion
3. `,,` + movement (e.g. `,,j`) and `,,w` for easy motion
4. `:set nobomb` to remove the byte order mark (BOM)
5. `ys`+text object+the thing you want to surround the text object with
    e.g.:`ysiw'` or `ysiw<b>` or `ysap(`. Warning: Be fast!
6. `cs`+old surround+new surround to change the surrounding, e.g. `cs'"` or
   `cst*` (t means (html) tag)
7. `ds`+surround to remove a surround, e.g. `ds"`
