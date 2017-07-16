This is the project for ionic-button

Buttons are an essential way to interact with and navigate through an app, and should clearly communicate what action will occur after the user taps them. Buttons can consist of text and/or an icon, and can be enhanced with a wide variety of attributes.

For accessibility reasons, buttons use a standard <button> element, but are enhanced with an ion-button directive.

There are several types of basic usage for button.

## Example

1. Basic Usage
The color property sets the color of the button. Ionic includes a number of default colors which can be easily overridden:

```<button ion-button color="light">Light</button>
<button ion-button>Default</button>
<button ion-button color="secondary">Secondary</button>
<button ion-button color="danger">Danger</button>
<button ion-button color="dark">Dark</button>
```

2. Outline Style
To use the outline style for a button, just add the outline property:

```
<button ion-button color="light" outline>Light Outline</button>
<button ion-button outline>Primary Outline</button>
<button ion-button color="secondary" outline>Secondary Outline</button>
<button ion-button color="danger" outline>Danger Outline</button>
<button ion-button color="dark" outline>Dark Outline</button>
```
3. Clear Style
To use the clear style for a button, just add the clear property:

```<button ion-button color="light" clear>Light Clear</button>
<button ion-button clear>Primary Clear</button>
<button ion-button color="secondary" clear>Secondary Clear</button>
<button ion-button color="danger" clear>Danger Clear</button>
<button ion-button color="dark" clear>Dark Clear</button>
```

4. Round Buttons
To create a button with rounded corners, just add the round property:

```
<button ion-button color="light" round>Light Round</button>
<button ion-button round>Primary Round</button>
<button ion-button color="secondary" round>Secondary Round</button>
<button ion-button color="danger" round>Danger Round</button>
<button ion-button color="dark" round>Dark Round</button>
```

5. Block Buttons
Adding block to a button will make the button take 100% of its parent’s width. It will also add display: block to the button:
```
<button ion-button block>Block Button</button>
```

6. Full Buttons
Adding full to a button will also make the button take 100% of its parent’s width. However, it will also remove the button’s left and right borders. This style is useful when the button should stretch across the entire width of the display.
```
<button ion-button full>Full Button</button>
```

7. Button Sizes
Add the large attribute to make a button larger, or small to make it smaller:

```
<button ion-button small>Small</button>
<button ion-button>Default</button>
<button ion-button large>Large</button>
```

8. Icon Buttons
To add icons to a button, add an icon component inside of it and a position attribute:

```
<!-- Float the icon left -->
<button ion-button icon-left>
  <ion-icon name="home"></ion-icon>
  Left Icon
</button>

<!-- Float the icon right -->
<button ion-button icon-right>
  Right Icon
  <ion-icon name="home"></ion-icon>
</button>

<!-- Only icon (no text) -->
<button ion-button icon-only>
  <ion-icon name="home"></ion-icon>
</button>
```

9. Buttons In Components
Although buttons can be used on their own, they can easily be used within other components. For example, buttons can be added to a list item or a navbar.
```
<ion-header>
  <ion-navbar>
    <ion-buttons start>
      <button ion-button icon-only>
        <ion-icon name="contact"></ion-icon>
      </button>
    </ion-buttons>

    <ion-buttons end>
      <button ion-button icon-only>
        <ion-icon name="search"></ion-icon>
      </button>
    </ion-buttons>
  </ion-navbar>
</ion-header>

<ion-list>
  <ion-item>
    Left Icon Button
    <button ion-button outline item-end icon-left>
      <ion-icon name="star"></ion-icon>
      Left Icon
    </button>
  </ion-item>
</ion-list>
```
