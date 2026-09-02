# seating_chart_builder

Build a seating chart: paste a guest list, drag names onto tables, arrange the room.

**Live: https://dsiegel.github.io/seating_chart_builder/**

The whole app is one file — `index.html`. No build, no server, no dependencies (aside from Google Fonts). Open it from the link above or straight off disk.

## Loading guests

Open **Guest data** and paste CSV or TSV — one row per guest or couple:

```
guest, companion, group
Jane Doe, John Doe, Table 1
Sam Rivera, , Table 1
Ada Lovelace
```

Companion and group are both optional. A row with no group starts out unseated; a row with a group but no name registers an empty table. A header row is skipped automatically. Loading replaces the current chart, and **Revert to last load** rebuilds the chart from the text you last pasted, discarding seating changes made since.

## Seating guests

Drag a name onto a table and the guests already there shuffle aside to show which seat it will take. Drag it back to the **Unseated** strip to take it out of the room. Tables past a dozen guests seat them in two rings.

Couples share a colored dot and a dashed line between the two halves, so a pair split across the room is easy to spot. Hovering a name outlines their companion.

## Tables

**+ Add table** adds one, clicking a table's name renames it, and **✕** removes it — its guests go back to Unseated. A table named with a bare number reads as "Table 7".

## Arrangements

Pick **Grid** (automatic columns, or 1–8), **Circle**, **Rectangle**, or **Custom**. In a preset arrangement, dragging a table reorders it through the arrangement's slots and the others slide around it — the table list, and so the exports, follow the order of the room. **Custom** drops the slots and lets you place each table wherever you like. A wide room scales down to fit the window, and scrolls sideways once it can't shrink further.

## Exporting

From the Guest data drawer:

- **CSV** / **TSV** — the chart as `guest, companion, group`, empty tables included, so it pastes straight back into the box. A couple seated at two different tables is written at the first partner's table.
- **Seat list** — a flat `group, seat, guest` export for place cards.

## Charts and sharing

Charts are saved in your browser. The **Charts** drawer on the left switches between them, starts a new one, or deletes one; each chart is named by its title in the top bar, and switching saves the chart you are leaving.

**Copy link** carries a chart to another browser or device — the whole chart travels inside the link. Opening one adds it as a new chart rather than overwriting anything already saved locally.

Light and dark follow your system theme.
