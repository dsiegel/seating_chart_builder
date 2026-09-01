# Layout features

- [x] Different table arrangements — grid (1–8 columns or auto), circle, and
      rectangle. Picking one in the toolbar slides the tables into place.
- [x] Drag a whole table to reposition it. Doing so switches the arrangement to
      Custom and keeps the hand-placed positions.
- [x] While a guest is being dragged, the people already at the table shuffle
      aside to open the seat the guest would land in.

## Ideas not done yet

- Snap or nudge tables apart when a hand-placed one is dropped on top of another.
- Reorder the underlying table list to match a custom layout, so exports read in
  the order the room is laid out.
- Zoom and pan the canvas instead of only auto-fitting it to the window.
- Wrap the canvas in a sizer div so a scaled-down board's scroll region matches
  what is drawn; today a ring big enough to hit the 0.3 scale floor scrolls a
  little way past its own tables.
