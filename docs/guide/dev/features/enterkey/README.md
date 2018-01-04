---
category: output-control
order: 60
url: guide/dev_enterkey
menu-title: Enter Key Configuration
meta-title-short: Enter Key Configuration
---
<!--
Copyright (c) 2003-2017, CKSource - Frederico Knabben. All rights reserved.
For licensing, see LICENSE.md.
-->

# Enter Key Configuration

When CKEditor is integrated in some environments you may want to configure the default behavior of the <kbd>Enter</kbd> and <kbd>Shift+Enter</kbd> keys to generate matching output. This is possible thanks to CKEDITOR.config.enterMode and CKEDITOR.config.shiftEnterMode, respectively.

Both configuration settings can use one of the following options:

* CKEDITOR.ENTER_P &ndash; new `<p>` paragraphs are created;
* CKEDITOR.ENTER_BR &ndash; lines are broken with `<br>` elements;
* CKEDITOR.ENTER_DIV &ndash; new `<div>` blocks are created.

<info-box hint="">
</info-box>

## Enter Key Configuration Demo

See the [working "Enter Key Configuration" sample](https://sdk.ckeditor.com/samples/enterkey.html) that showcases the effects of using different settings for <kbd>Enter</kbd> and <kbd>Shift+Enter</kbd> keys on editor output.
</div></br></p>