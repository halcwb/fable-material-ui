# GridListTile

<p class="description">The API documentation of the GridListTile React component. Learn more about the properties and the CSS customization points.</p>

```fsharp
Fable.Helpers.MaterialUI.gridListTile (props : IHTMLProp list) (children : ReactElement list) : ReactElement
```



## Props

| Name | Type | Default | Description |
|:-----|:-----|:--------|:------------|
| <span class="prop-name">children</span> | <span class="prop-type">node</span> |   | Theoretically you can pass any node as children, but the main use case is to pass an img, in which case GridListTile takes care of making the image "cover" available space (similar to `background-size: cover` or to `object-fit: cover`). |
| <span class="prop-name">MaterialProp.Classes</span> | <span class="prop-type">ClassNames list</span> |   | Override or extend the styles applied to the component.  See CSS API below for more details.  |
| <span class="prop-name">cols</span> | <span class="prop-type">number</span> | <span class="prop-default">1</span> | Width of the tile in number of grid cells. |
| <span class="prop-name">MaterialProp.Component</span> | <span class="prop-type">ReactType</span> | <span class="prop-default">"li"</span> | The component used for the root node. Either a string to use a DOM element or a component. |
| <span class="prop-name">rows</span> | <span class="prop-type">number</span> | <span class="prop-default">1</span> | Height of the tile in number of grid cells. |

Any other properties supplied will be spread to the root element (native element).

## CSS API

You can override all the class names injected by Material-UI thanks to the `MaterialProp.Classes` property.
This property accepts the following keys:


| Name | Description |
|:-----|:------------|
| <span class="prop-name">ClassNames.Root</span> | Styles applied to the root element.
| <span class="prop-name">ClassNames.Tile</span> | Styles applied to the `div` element that wraps the children.
| <span class="prop-name">ClassNames.ImgFullHeight</span> | Styles applied to an `img` element child, if needed to ensure it covers the tile.
| <span class="prop-name">ClassNames.ImgFullWidth</span> | Styles applied to an `img` element child, if needed to ensure it covers the tile.

Have a look at [overriding with classes](#/customization/overrides) section
and the [implementation of the component](https://github.com/mui-org/material-ui/tree/master/packages/material-ui/src/GridListTile/GridListTile.js)
for more detail.

If using the `overrides` key of the theme as documented
[here](#/customization/themes),
you need to use the following style sheet name: `OverridesProp.MuiGridListTile`.

## Demos

- [Grid List](/demos/grid-list/)
