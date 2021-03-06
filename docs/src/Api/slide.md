# Slide

<p class="description">The API documentation of the Slide React component. Learn more about the properties and the CSS customization points.</p>

```fsharp
Fable.MaterialUI.Core.slide (props : seq<IHTMLProp>) (children : seq<ReactElement>) : ReactElement
```

The Slide transition is used by the [Snackbar](#/api/snackbars/) component.
It uses [react-transition-group](https://github.com/reactjs/react-transition-group) internally.

## Props

| Name | Type | Default | Description |
|:-----|:-----|:--------|:------------|
| <span class="prop-name">SlideProp.Direction</span> | <span class="prop-type">type&nbsp;SlideDirection&nbsp;=<br>&nbsp;&nbsp;&#124;&nbsp;Bottom<br>&nbsp;&nbsp;&#124;&nbsp;Up<br>&nbsp;&nbsp;&#124;&nbsp;Left<br>&nbsp;&nbsp;&#124;&nbsp;Right<br></span> | <span class="prop-default">SlideDirection.Down</span> | Direction the child node will enter from. |
| <span class="prop-name">MaterialProp.In</span> | <span class="prop-type">bool</span> |   | If `true`, show the component; triggers the enter or exit animation. |
| <span class="prop-name">MaterialProp.Timeout</span> | <span class="prop-type">U2&lt;float,&nbsp;TransitionDurationProp&nbsp;list&gt;<br><br>type&nbsp;TransitionDurationProp&nbsp;=<br>&nbsp;&nbsp;&#124;&nbsp;Enter&nbsp;of&nbsp;float<br>&nbsp;&nbsp;&#124;&nbsp;Exit&nbsp;of&nbsp;float<br></span> | <span class="prop-default">{  enter: duration.enteringScreen,  exit: duration.leavingScreen,}</span> | The duration for the transition, in milliseconds. You may specify a single timeout for all transitions, or individually with an object. |

Any other properties supplied will be spread to the root element ([Transition](https://reactcommunity.org/react-transition-group/#Transition)).

## Inheritance

The properties of the [Transition](https://reactcommunity.org/react-transition-group/#Transition) component, from react-transition-group, are also available.
<!-- You can take advantage of this behavior to [target nested components](/guides/api/#spread). -->

<!--## Demos-->

<!--- [Dialogs](/demos/dialogs/)-->
<!--- [Transitions](/utils/transitions/)-->

