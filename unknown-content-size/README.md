# Unknown Content Size

If you know how many items you will have but do not know the amount of content that will be in each, you can use either Flexbox or Grid.

## Flexbox

```css
.known {
  margin: 100px 0;
  display: flex;
  justify-content: center;
}

.known > * {
  margin: 20px;
}
```

## CSS Grid

```css
.known {
  margin: 100px 0;
  display: grid;
  grid-template-columns: repeat(5, auto);
  justify-content: center;
  grid-gap: 20px;
}
```

![Screenshot of unknown content size](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551214647/Screenshot_2019-02-26_Flexbox_vs_CSS_Grid_Unknown_Content_Size_had5fi.png)
