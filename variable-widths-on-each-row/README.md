# Variable Widths on Each Row

Flexbox allows you to have variable widths on each row using `flex-wrap` and setting each item to `flex: 1`.

As Flexbox doesn't have a gap property, you can't evenly space the items and have the first and last item on each row line up with the edge of the container.

With Grid, you would have to manually span each item to achieve a layout like this.

```css
.flex-container {
  display: flex;
  flex-wrap: wrap;
  border: 3px solid var(--yellow);
}

.flex-container > * {
  margin: 10px;
  flex: 1;
}
```

![Screenshot of various widths on each row example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1550927773/Screenshot_2019-02-23_Flexbox_vs_CSS_Grid_Variable_Widths_on_Each_Row_ejrb1z.png)
