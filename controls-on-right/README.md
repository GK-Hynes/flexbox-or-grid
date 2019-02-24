# Controls on the right

Both Flexbox and Grid could be used where you want to one item to take up most of the space with any other items fitted in on the end. For example, the controls on a media player.

## Flexbox

Set the desired item to `flex: 1` and it will grow to take up all the space not taken up by the others.

## CSS Grid

With Grid, set the grid to be one column wide. By default the controls will be pushed onto the next rows.

By using `grid-auto-flow: column`, however, you can tell Grid to add them as new implcit columns at the end of the explicit column.

```css
.track {
  background: white;
  padding: 10px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  display: grid;
  grid-template-columns: 1fr;
  grid-auto-flow: column;
}
```

![Screenshot of controls on right example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551029065/Screenshot_2019-02-24_Flexbox_vs_CSS_Grid_Controls_on_Right_1_pdriwy.png)
