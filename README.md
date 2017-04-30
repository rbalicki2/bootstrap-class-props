# Bootstrap Class Props

> A decorator which adds props like `textMuted` to components

## Usage

### With external components
```
import addBootstrapClassProps from 'bootstrap-class-props';
import SomeExistingComponent from './MyComponent';
export default addBootstrapClassProps(SomeExistingComponent);
```

### With components defined in the file
```
import React, { Component } from 'react';
import addBootstrapClassProps from 'bootstrap-class-props';

@addBootstrapClassProps
export default class MyComponent extends Component {}
```

Now, `MyComponent` and `SomeExistingComponent` have props like `bgSuccess`, etc. These props, if present and truthy,
add the appropriate className to the component.

## Full list of props and utility classes

The keys in this object are the prop names. The values are the classes applied.

```
{
  "textMuted": "text-muted",
  "textPrimary": "text-primary",
  "textSuccess": "text-success",
  "textInfo": "text-info",
  "textWarning": "text-warning",
  "textDanger": "text-danger",
  "bgPrimary": "bg-primary",
  "bgSuccess": "bg-success",
  "bgInfo": "bg-info",
  "bgWarning": "bg-warning",
  "bgDanger": "bg-danger",
  "pullLeft": "pull-left",
  "pullRight": "pull-right",
  "navbarLeft": "navbar-left",
  "navbarRight": "navbar-right",
  "centerBlock": "center-block",
  "clearfix": "clearfix",
  "invisible": "invisible",
  "srOnly": "sr-only",
  "srOnlyFocusable": "sr-only sr-only-focusable",
  "textHide": "text-hide",
  "visibleXsBlock": "visible-xs-block",
  "visibleXsInline": "visible-xs-inline",
  "visibleXsInlineBlock": "visible-xs-inline-block",
  "hiddenXs": "hidden-xs",
  "visibleSmBlock": "visible-sm-block",
  "visibleSmInline": "visible-sm-inline",
  "visibleSmInlineBlock": "visible-sm-inline-block",
  "hiddenSm": "hidden-sm",
  "visibleMdBlock": "visible-md-block",
  "visibleMdInline": "visible-md-inline",
  "visibleMdInlineBlock": "visible-md-inline-block",
  "hiddenMd": "hidden-md",
  "visibleLgBlock": "visible-lg-block",
  "visibleLgInline": "visible-lg-inline",
  "visibleLgInlineBlock": "visible-lg-inline-block",
  "hiddenLg": "hidden-lg",
  "visiblePrintBlock": "visible-print-block",
  "visiblePrintInline": "visible-print-inline",
  "visiblePrintInlineBlock": "visible-print-inline-block",
  "hiddenPrint": "hidden-print",
  "textLeft": "text-left",
  "textCenter": "text-center",
  "textRight": "text-right",
  "textJustify": "text-justify",
  "textNowrap": "text-nowrap",
  "textLowercase": "text-lowercase",
  "textUppercase": "text-uppercase",
  "textCapitalize": "text-capitalize",
  "initialism": "initialism"
}
```

## My favorite bootstrap classes are omitted!

I omitted classes like `show`, `hidden`, `caret` and `close` because they are way too generic and will conflict with existing props.

I omitted classes like `lead`, `blockquote-reverse`, etc. because they are too component-specific.

If you want to add these back, a future release will give you that ability!

## TODO

* Expose an easy way of adding props for classes you custom-defined.
* Tests
* Typescript bindings?

## Contributing

Please, feel free to reach out and contribute! [robert.balicki@gmail.com](mailto:robert.balicki@gmail.com)
