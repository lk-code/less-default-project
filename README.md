# LESS Default Project

This is a default structure, inspired by Shopware.

## Getting Started

You only have to integrate the file all.less.

---

## Structure

### *plugins*

add additional plugins style here. add the file in the plugins.less in the root directory.

### *variables*

add your project variables here. There are already some examples:

* color.less - contains some color variables.
* structure.less - contains variables for media queries.

### *mixins*

add your individual mixins here.

#### transition.less

##### usage
```
.transition ( all, 0.25s, ease );
```

##### output
```
-webkit-transition: all, 0.25s, ease;
-moz-transition: all, 0.25s, ease;
-ms-transition: all, 0.25s, ease;
-o-transition: all, 0.25s, ease;
transition: all, 0.25s, ease;
```

#### iphone-x-device-padding.less

add css for the iphone-x save area (for the notch and the virtual home button). see more at https://webkit.org/blog/7929/designing-websites-for-iphone-x/

##### usage
```
.iphonex-padding-all (); // add all 3 styles
.iphonex-padding-left ();
.iphonex-padding-right ();
.iphonex-padding-bottom ();
```

---

### *components*

add your style for components like buttons, links, images, etc. here.

### *components/fonts*

you can add your own webfonts (and icon fonts :D) here. the webfont 'Open-Sans' is already added. on the same way you can add every other web and icon font.

#### Open-Sans

in the style.less for Open-Sans is the complete css code from google fonts. in the first lines there is a mixin for add the font-family value for Open-Sans on any position.

##### usage
```
.set-font-open-sans();
```

##### output
```
font-family: 'Open Sans', sans-serif;
```

---

### *modules*

add your style for modules like pages or specific content like login-forms, etc. here.