---
title: Button
slug: gs-mobile-button
tags: getting-started,mobile
publish: true
---

# Button

The mobile Button widget navigates to mobile View or executes a custom callback when tapped.

## Getting Started

The Kendo mobile Application will automatically initialize a mobile Button widget for every element with `role` data attribute set to `button` present in the views/layouts' markup.
Alternatively, it can be initialized using jQuery plugin syntax in the containing mobile View **init event handler**.
The button element may be either `A` or `BUTTON`.

### Initialize Kendo mobile Button based on role data attribute

    <a href="#foo" data-role="button">Foo</a>

### Initialize Kendo mobile Button using jQuery

    var button = $("#button").kendoMobileButton();

## Customizing Mobile Button Appearance

The Kendo mobile Button color can be customized by setting its `background-color` CSS property inline or by using a CSS selector with specificity of 20+.
You can target platforms separately using their respective root CSS classes.

### Green Button

    <a href="#foo" data-role="button" style="background-color: green">Foo</a>

### Green Kendo mobile Button in iOS and a red one in Android

    <style>
        .km-ios .checkout { background-color: green; }
        .km-android .checkout { background-color: red; }
    </style>

    <a href="#foo" data-role="button" class="checkout">Foo</a>

## Button icons

A Button icon can be set in two ways - either by adding an `img` element inside the Button element,
or by setting an `icon` data attribute to the Button element.

KendoUI Mobile ships with several ready to use icons:

*   <span class="km-icon km-about"></span>about
*   <span class="km-icon km-action"></span>action
*   <span class="km-icon km-add"></span>add
*   <span class="km-icon km-bookmarks"></span>bookmarks
*   <span class="km-icon km-camera"></span>camera
*   <span class="km-icon km-cart"></span>cart
*   <span class="km-icon km-compose"></span>compose
*   <span class="km-icon km-contacts"></span>contacts
*   <span class="km-icon km-details"></span>details
*   <span class="km-icon km-downloads"></span>downloads
*   <span class="km-icon km-fastforward"></span>fastforward
*   <span class="km-icon km-favorites"></span>favorites
*   <span class="km-icon km-featured"></span>featured
*   <span class="km-icon km-toprated"></span>toprated
*   <span class="km-icon km-globe"></span>globe
*   <span class="km-icon km-history"></span>history
*   <span class="km-icon km-home"></span>home
*   <span class="km-icon km-info"></span>info
*   <span class="km-icon km-more"></span>more
*   <span class="km-icon km-mostrecent"></span>mostrecent
*   <span class="km-icon km-mostviewed"></span>mostviewed
*   <span class="km-icon km-organize"></span>organize
*   <span class="km-icon km-pause"></span>pause
*   <span class="km-icon km-play"></span>play
*   <span class="km-icon km-recents"></span>recents
*   <span class="km-icon km-refresh"></span>refresh
*   <span class="km-icon km-reply"></span>reply
*   <span class="km-icon km-rewind"></span>rewind
*   <span class="km-icon km-search"></span>search
*   <span class="km-icon km-settings"></span>settings
*   <span class="km-icon km-share"></span>share
*   <span class="km-icon km-stop"></span>stop
*   <span class="km-icon km-trash"></span>trash



Additional icons may be added by defining the respective CSS class.
If the `icon` data attribute is set to `custom`, the tab will receive `km-custom` CSS class.

## Creating Custom Icons

In order to create colorizable icons like the default ones in Kendo UI Mobile, specify the icon image as a **box mask**
(either as dataURI or as a separate image). The image should be **PNG8** or **PNG24** with alpha channel (**PNG8+Alpha** is supported by
only few graphic editors, so **better stick with PNG24**). The image color is not important - it will be used as a mask only.

**Note**: **BlackBerry 7.0** has a bug that renders its masks as background-image, so it is recommended to use white in order to support it. The bug is fixed in **7.1**.

### Define custom button icon

    <style>
        .km-custom {
          -webkit-mask-box-image: url("foo.png");
        }
    </style>

    <a data-role="button" href="#index" data-icon="custom">Home</a>

In Q3 2012 due to numerous issues with WebKit mask icons, they were deprecated and Kendo UI Mobile introduced font icons. Since the font is not easy editable,
the previous method for a mask icon can be used, but with some additional styling. Please note that the below example will restyle all font icons.

### Define custom button icon after Q3 2012

    <style>
        /* Remove font icons styling, use .km- + data-icon name if only one should be overridden */
        .km-root .km-pane .km-view .km-icon {
            background-size: 100% 100%;
            -webkit-background-clip: border-box;
            background-color: currentcolor;
        }

        .km-custom {
            -webkit-mask-box-image: url("foo.png");
            background-color: red;
        }
    </style>

    <a data-role="button" href="#index" data-icon="custom">Home</a>

If you want to add only one or two custom icons, specify them with their respective classes (.km- + data-icon name):

### Restyle only the added Kendo UI Mobile custom icon.

    .km-root .km-pane .km-view .km-question {
        background-size: 100% 100%;
        -webkit-background-clip: border-box;
        background-color: currentcolor;
    }

    .km-question {
        -webkit-mask-box-image: url("foo.png");
        background-color: red;
    }

When custom icons are used and their names are the same as the integrated Kendo UI Mobile icon names, make sure that the font icons are not rendered.

### Hide all Kendo UI Mobile font icons.

    /* Don't render all internal Kendo UI font icons
    .km-root .km-pane .km-view .km-icon:after,
    .km-root .km-pane .km-view .km-icon:before
    {
        visibility: hidden;
    }

Again if only several icons should be overridden, specify them with their classes instead:

### Hide specific Kendo UI Mobile font icons.

    .km-root .km-pane .km-view .km-favorites:after,
    .km-root .km-pane .km-view .km-favorites:before
    {
        visibility: hidden;
    }

