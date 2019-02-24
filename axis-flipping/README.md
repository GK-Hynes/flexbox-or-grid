# Axis Flipping

## Flexbox

With Flexbox, to switch a layout from columns to rows, just change `flex-direction`.

```css
.flipper.flip {
  flex-direction: column;
}
```

Flexbox can do `row-reverse` and `column-reverse`. You could do this with the order property in Grid but is is more of a hassle.

## CSS Grid

With Grid, to switch a layout from columns to rows, just make it one column wide.

```css
.flipper {
  display: grid;
  grid-gap: 20px;
  grid-template-columns: repeat(auto-fit, minmax(50px, 1fr));
}

.flipper.flip {
  grid-template-columns: 1fr;
}
```

![Screenshot of axis flipping example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551027962/Screenshot_2019-02-24_Flexbox_vs_CSS_Grid_Axis_Flipping_vl15g4.png)
