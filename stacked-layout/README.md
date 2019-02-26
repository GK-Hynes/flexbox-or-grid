# Stacked Layout

Staggered or stacked layouts are much easier in Flexbox.

Set `flex-wrap` to `wrap` and `justify-content` to `space-around`.

In Grid, the columns and rows are quite rigid and you would need to manually span items in order to stagger them.

One advantage of Grid is `grid-gap` which removes the need to mess around with negative margins.

```css
.stacked {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.stacked > * {
  width: 30%;
  margin-bottom: 20px;
}
```

![Screenshot of stacked layout example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551214105/Screenshot_2019-02-26_Flexbox_vs_CSS_Grid_Stacked_Layout_bidzqz.png)
