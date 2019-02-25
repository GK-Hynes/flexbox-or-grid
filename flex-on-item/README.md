# Flex on Item

If you want one item to take up all the free space, Flexbox is better than Grid.

## Flexbox

With Flexbox, you just set the desired item to `display: flex`

```css
.controls {
  display: flex;
}

.scrubber {
  flex: 1;
}
```

## CSS Grid

With Grid, you need to set all the other items to `auto` and the desired item to `1fr`.

This is more brittle as it depends on knowing in advance both the order and number of items.

```css
.controls {
  display: grid;
  grid-template-columns: auto auto auto 1fr auto auto;
}
```

![Screenshot of flex on item example](https://res.cloudinary.com/gerhynes/image/upload/q_auto/v1551126740/Screenshot_2019-02-25_Flexbox_vs_CSS_Grid_Flex_on_Item_eow3qs.png)
