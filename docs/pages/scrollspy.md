# Scrollspy

<p class="uk-text-lead">Trigger events and animations while scrolling your page.</p>

## Usage

The Scrollspy component listens to page scrolling and triggers events based on the scroll position. For example, if you scroll down a page and an element appears in the viewport for the first time, you can trigger a smooth animation to fade in the element. Just add the `uk-scrollspy` attribute and the following options.

| Data attribute | Description |
| -------------- | ----------- |
| `cls:'MY-CLASS'` | Applies the class only the first time the element appears in the viewport. |
| `repeat: true` | Applies the class every time the element appears in the viewport. |
| `delay:600` | Adds a delay in milliseconds to the animation. |

Typically, classes from the [Animation component](animation.md) are used together with the scrollspy component.

```html
<div uk-scrollspy="cls:uk-animation-fade"></div>
```

```example
<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-fade; repeat: true">
    <h3>Fade</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>

<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-scale-up; repeat: true">
    <h3>Scale up</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>

<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-scale-down; repeat: true">
    <h3>Scale down</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>

<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-slide-top; repeat: true">
    <h3>Slide top</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>

<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-slide-bottom; repeat: true">
    <h3>Slide bottom</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>

<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-slide-right; repeat: true">
    <h3>Slide right</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>

<div class="uk-card uk-card-default uk-card-body uk-margin" uk-scrollspy="cls:uk-animation-slide-left; repeat: true">
    <h3>Slide left</h3>
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
</div>
```

This example uses the `repeat: true` option. Scroll up and down to see the triggered animations. The layout is made with the [Card component](card.md).

***

## Groups

You can also group scrollspy elements, so you won't have to apply the attribute to each of them. Just add the `uk-scrollspy="target:MY-CLASS"` attribute to a container element, targeting the selector of the items you want to animate inside the container. When using a delay, it will be applied cumulatively to the items within the row that scrolls into view. The delay will be reseted for the next row within the group when it scrolls into view.

```html
<div uk-scrollspy="target: > div; cls:uk-animation-fade">
    <div></div>
    <div></div>
</div>
```

```example
<div class="uk-child-width-1-4@m" uk-grid uk-scrollspy="cls: uk-animation-fade; target: > div > .uk-card; repeat: true">
    <div>
        <div class="uk-card uk-card-default uk-card-body">
            <h3 class="uk-card-title">Fade</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">
            <h3 class="uk-card-title">Fade</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">
            <h3 class="uk-card-title">Fade</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
    </div>
    <div>
        <div class="uk-card uk-card-default uk-card-body">
            <h3 class="uk-card-title">Fade</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
    </div>
</div>
```

***

## Scrollspy Nav

To automatically update the active menu item in a menu depending on the scroll position of your site, just add the `uk-scrollspy-nav` attribute to any navigation. Each menu item must link to the ID of its corresponding part of the site.

| Data attribute | Description|
| --- | --- |
| `uk-scrollspy-nav` | Triggers the JavaScript necessary for the functionality of the scrollspy nav.|
| `uk-scrollspy-nav="closest:MY-SELECTOR"` | Looks for the closest element that matches the selector by testing the element itself and traversing up through its ancestors in the DOM tree.|
| `uk-scrollspy-nav="scroll:true"` | Applies the [Scroll component](scroll.md) when skipping between different sections of the site.|
| `uk-scrollspy-nav="cls:MY-CLASS"` | By default ScrollspyNav toggles the uk-active class. Use the cls option to use your own class name.|

For an example of the scrollspy nav, just check out our [Scrollspy test page](http://www.getuikit.com/tests/scrollspy.html).

| Option | Value | Default | Description |
| --- | --- | --- | --- |
| `cls` | String | uk-active | Class to add to the active links. |
| `closest` | String | uk-scrollspy-init-inview | Target to apply the class to. |
| `scroll` | Boolean | false | Adds the [Scroll component](scroll.md) to its links. |
| `overflow` | Boolean | true | If overflow is set to true, the first or last item will stay active if above or below the navigation. |

***

## Component options

| Option | Value | Default | Description |
| --- | --- | --- | --- |
| `cls` | String | uk-scrollspy-inview | Class to add when the element is in view. If two, comma separated classes are provided those will be toggled. |
| `hidden` | Boolean | true | Hides the element while out of view. |
| `offset-top` | Number | 0 | Top offset before triggering in view. |
| `offset-left` | Number | 0 | Left offset before triggering in view. |
| `repeat` | Boolean | false | Applies the 'cls' class every time the element is in view. |
| `delay` | Number | 0 | Delay time in ms. |