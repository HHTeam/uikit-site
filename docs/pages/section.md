# Section

<p class="uk-text-lead">Create horizontal layout sections with different background colors and styles.</p>

## Usage

To apply this component, just add the `.uk-section` class to a container element.

```html
<div class="uk-section"></div>
```

```example
<div class="uk-section uk-section-muted">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>
```

***

## Color Modifiers

To apply different background colors and paddings, add one of the following classes. If two consecutive blocks have the same background color, the padding will automatically be divided.

| Class                 | Description                                                  |
|-----------------------|--------------------------------------------------------------|
| `.uk-section-default` | Adds the default background color, usually white or similar. |
| `.uk-section-muted`   | Adds a light background color.                               |
| `.uk-section-primary` | Adds a primary background color.                             |
| `.uk-section-primary` | Adds a another background color, usually a dark one.         |

```html
<div class="uk-section uk-section-primary"></div>
```

Note: To properly display colors, borders and other elements on colored sections, you might want to apply the `.uk-light` class from the [Inverse component](inverse.md).

```example
<div class="uk-section uk-section-default">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Default</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>

<div class="uk-section uk-section-muted">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Muted</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>

<div class="uk-section uk-section-primary uk-light">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Primary</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>

<div class="uk-section uk-section-secondary uk-light">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Secondary</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>
```

***

## Section Media

When using a section with a background image, add the `.uk-section-media` class.

```html
<div class="uk-section uk-section-media"></div>
```

```example
<div class="uk-section uk-section-media uk-light uk-background-cover" style="background-image: url(../docs/images/dark.jpg)">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Media</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>
```

***

## Padding

You can add different paddings to each section or remove it altogether.

### Small

To decrease a section's padding, add the `.uk-section-small` class.

```example
<div class="uk-section uk-section-small uk-section-muted">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Small</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>
```

***

### Large

To increase a section's padding, add the `.uk-section-large` class.

```example
<div class="uk-section uk-section-large uk-section-muted">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Section Large</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>
```

***

### Remove Padding

To remove a section's padding, add the `.uk-padding-remove-vertical` class from the [Padding component](padding.md).

```example
<div class="uk-section uk-section-muted uk-padding-remove-vertical">
    <div class="uk-margin-small-left uk-margin-small-right">

        <h3>Remove Padding</h3>

        <div class="uk-grid-match uk-child-width-1-3@m uk-grid-small" uk-grid>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
            <div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
            </div>
        </div>
    </div>
</div>
```