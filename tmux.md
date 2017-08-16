# tmux tips

## Show a clock

`prefix + t` puts a clock in the current pane. Press any key to continue.

## Creating windows

`prefix + c` makes a new (empty) window. To put the current pane in a new (its
own) window, `prefix+!` does the job.

## Zooming into a pane

`prefix + z` makes the current pane as big the current window (temporarily).
Same to zoom out.

## Copying text

`prefix + ^C` copies whats currently in the buffer to the system clipboard. The tmux buffer automatically gets filled by what is being selected with the mouse.

1. Select text with the mouse
2. Press `prefix + ^C`.
3. Press ⌘V elsewhere.
