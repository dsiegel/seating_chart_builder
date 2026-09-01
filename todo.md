# Layout features

- [x] Different table arrangements — grid (1–8 columns or auto), circle, and
      rectangle. Picking one in the toolbar slides the tables into place.
- [x] Drag a whole table to move it. In a preset arrangement the card snaps into
      the arrangement's slots and the tables it passes slide out of the way;
      the Custom arrangement is the one that takes a free, hand-placed position.
- [x] Reorder the underlying table list to match the layout, so exports read in
      the order the room is laid out.
- [x] While a guest is being dragged, the people already at the table shuffle
      aside to open the seat the guest would land in.
- [x] Animate the shuffling — seated chips transition to their new seats, and
      the unseated strip's flow layout is played back with FLIP.

## Ideas not done yet

- Animate adding and removing a table, which still reflows the board in one jump.
- Zoom and pan the canvas instead of only auto-fitting it to the window.
- Wrap the canvas in a sizer div so a scaled-down board's scroll region matches
  what is drawn; today a ring big enough to hit the 0.3 scale floor scrolls a
  little way past its own tables.
