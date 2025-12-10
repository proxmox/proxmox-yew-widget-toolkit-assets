<link rel="stylesheet" type="text/css" href="css/desktop-yew-style.css" />
<link rel="stylesheet" type="text/css" href="css/font-awesome.css" />
<link rel="stylesheet" type="text/css" href="css/doc-style.css" />

<style>
    .doc-example {
        padding: var(--pwt-spacer-2);
        margin-block: var(--pwt-spacer-2);
        border: 1px solid var(--pwt-color-border);
        border-radius: var(--pwt-shape-corner-medium);
    }
</style>


# Button Widget

The button widget is used to trigger actions. The `pwt-button` class is the top level class for the button widget.

Buttons have the following features:

- use color scheme variables
- font `label-large`
- use elevation and ripple effect

## Layout Options

There are several layout options available, suited for different use cases.

### Filled Button

This is the default style, using the `surface` color scheme.

```html
<button class="pwt-button">
    Setting
</button>
```

<div class="doc-example">
    <button class="pwt-button">
        Setting
    </button>
</div>

### Text Button

Text buttons are typically used for less pronounced actions, including those located in dialogs and cards. In cards, text buttons help maintain an emphasis on card content.

Use the `pwt-button-text` class to create a text button.

```html
<button class="pwt-button pwt-button-text">
    Save
</button>
```

<div class="doc-example">
    <button class="pwt-button pwt-button-text">
        Save
    </button>
</div>

### Outline Button

Outlined buttons are medium-emphasis buttons. They contain actions that are important but aren't the primary action in an app.

Use the `pwt-button-outline` class.

```html
<button class="pwt-button pwt-button-outline">
    Cancel
</button>
```

<div class="doc-example">
    <button class="pwt-button pwt-button-outline">
        Cancel
    </button>
</div>

### Elevated Button

Elevated buttons are essentially filled buttons that have a shadow.

Use the `pwt-button-elevated` class.

```html
<button class="pwt-button pwt-button-elevated">
    Upload
</button>
```

<div class="doc-example">
    <button class="pwt-button pwt-button-elevated">
        Upload
    </button>
</div>

### Segmented Button

Segmented buttons allow users to toggle the selected state of a single or multiple items. Use the `pwt-segmented-button` wrapper class.

> [!WARNING]
> Buttons are `inline-flex` elements. Thus, any whitespace between the button tags in the source code will be rendered as space between the buttons. To avoid this, make sure there is no whitespace between the tags.

#### Outline Segmented Button

Use the `pwt-button-outline` class on the container.

```html
<div class="pwt-segmented-button pwt-button-outline rounded">
    <button class="pwt-button">Day</button><button class="pwt-button pressed">Week</button><button class="pwt-button">Month</button><button class="pwt-button">Year</button>
</div>
```

<div class="doc-example">
    <div class="pwt-segmented-button pwt-button-outline rounded">
        <button class="pwt-button">Day</button><button class="pwt-button pressed">Week</button><button class="pwt-button">Month</button><button class="pwt-button">Year</button>
    </div>
</div>

#### Elevated Segmented Button

Use the `pwt-button-elevated` class on the container.

```html
<div class="pwt-segmented-button pwt-button-elevated rounded">
    <button class="pwt-button">Day</button><button class="pwt-button pressed">Week</button><button class="pwt-button">Month</button><button class="pwt-button">Year</button>
</div>
```

<div class="doc-example">
    <div class="pwt-segmented-button pwt-button-elevated rounded">
        <button class="pwt-button">Day</button><button class="pwt-button pressed">Week</button><button class="pwt-button">Month</button><button class="pwt-button">Year</button>
    </div>
</div>

### Buttons with Icons

Buttons can include icons.

```html
<button class="pwt-button">
    <i class="fa fa-refresh"></i> Refresh
</button>
```

<div class="doc-example">
    <button class="pwt-button">
        <i class="fa fa-refresh"></i> Refresh
    </button>
</div>

```html
<button class="pwt-button pwt-button-text">
    <i class="fa fa-trash-o"></i> Remove
</button>
```

<div class="doc-example">
    <button class="pwt-button pwt-button-text">
        <i class="fa fa-trash-o"></i> Remove
    </button>
</div>
