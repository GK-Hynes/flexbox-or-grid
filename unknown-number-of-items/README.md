# Unknown Number of Items

Both Flexbox and Grid can handle an unknown number of items but Grid allows you to be slightly more flexbible by using `auto-fit` and `minmax()`.

## Flexbox

```css
.unknown {
  display: flex;
  flex-wrap: wrap;
}

.unknown > * {
  width: 50px;
  margin: 20px;
}
```

## CSS Grid

```css
.unknown {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(50px, 1fr));
  grid-gap: 20px;
}
```

![Screenshot of unknown number of items example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551215360/Screenshot_2019-02-26_Flexbox_vs_CSS_Grid_Unknown_Number_of_Items_yb1ofp.png)
