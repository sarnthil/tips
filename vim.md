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
8. `:s/123-\zs456\ze-789/000` set the match for replacement to be between `\zs` and `\ze` 
9. `:help /\zs` opens the help page for the regex tip described in 8. 
10. `"_cw^R"` substitute a word with some other in your register. a bit too complex, and fun. 

```
foo
bar bay bat

"_c(text object)^R"
"_cw^R"
         sequence
          /      \
     N-change    I-registerpaste
     /    |        |
 toreg  word    default-register
   |
blackhole
```

11. 
