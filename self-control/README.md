# Self Control

If you want to align items to all four corners of a container, you'll need to use CSS Grid.

While Flexbox has `align-self`, Grid also has `justify-self`.

Here the items are positioned in the bottom right corner of each cell using `align-items: end` and `justify-items: end`.

You can then use `align-self: start` and `justify-self: start` to overwrite this and push the selected items to the top or left.

```css
.corners {
  display: grid;
  height: 200px;
  width: 200px;
  border: 10px solid var(--yellow);
  grid-template: 1fr 1fr / 1fr 1fr;
  align-items: end;
  justify-items: end;
}

.corner:nth-child(1),
.corner:nth-child(2) {
  align-self: start;
}

.corner:nth-child(1),
.corner:nth-child(3) {
  justify-self: start;
}
```

![Screenshot of self-control example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551127550/Screenshot_2019-02-25_Flexbox_vs_CSS_Grid_Self_Control_msfylc.png)
