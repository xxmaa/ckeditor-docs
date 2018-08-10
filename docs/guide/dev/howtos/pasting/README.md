---
category: howtos
order: 140
url: guide/dev_howtos_pasting
menu-title: Pasting
meta-title-short: Pasting
---
<!--
Copyright (c) 2003-2018, CKSource - Frederico Knabben. All rights reserved.
For licensing, see LICENSE.md.
-->

# Pasting

The following article contains tips about customizing the pasting behavior of CKEditor.


## How Do I Preserve Font Styles and Backgrounds When Pasting from Word?

The {@link guide/dev/features/pastefromword/README Paste from Word} feature lets you copy the content of Microsoft Word or Excel documents and paste them into the editor, preserving the structure and styles that were present in the original text.

Note, however, that by default some font styles are not preserved to avoid conflicting with the styles of the document created in CKEditor. If however, you want to use Word font styles, including font size, font family, and font foreground/background color, set the {@linkapi CKEDITOR.config#pasteFromWordRemoveFontStyles CKEDITOR.config#pasteFromWordRemoveFontStyles} configuration value to `false`.

	config.pasteFromWordRemoveFontStyles = false;

Please note that since CKEditor 4.1 you need to add {@link guide/dev/acf/README Advanced Content Filter} into the equation, too. The content filtering mechanism makes sure that the data that enters the editor is supported by editor features that are enabled in your configuration (to simplify it: if there is no font or text/background color button in your toolbar, this formatting will be stripped from your Word-formatted text). ACF is a highly flexible tool, though, so you can {@linksdk acf easily adjust it to your needs}.
