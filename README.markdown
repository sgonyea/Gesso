Gesso
=====

Gesso is best described as a primer coat for a CSS project; more than a CSS Reset and less than a CSS Framework.

Usage
----- 

From the head of an HTML or XHTML document reference the layout.css (screen media) and print.css (print media) files and, if necessary, the ie7.css and/or ie6.css stylesheet using conditional comments. 

These styles are designed to work best with an XHTML 1.0 Strict Doctype and a semantics-based design technique. The package uses a normalizing stylesheet and the `<address>`, `<b>`, `<big>`, `<caption>`, `<cite>`, `<code>`, `<dfn>`, `<em>`, `<i>`, `<small>`, `<strong>`, `<th>`, `<u>`, and `<var>` elements have their default styling completely removed. Other elements are mostly reset.

`<div>` is treated as a purely structural element and lists are setup to require styling to serve as textual lists.

The Typography stylesheet sets up a Baseline Grid and defines screen-friendly font stacks including a humanist sans-serif stack, a serif stack and a monospace font stack.

There are a few extra non-semantic hooks for better typographic styling including a definition for the .amp class (for ampersands customization) and a .caps class definition for setting text in all caps.

The effects of these stylesheets and the methods used to import them can and will have odd effects (or just flat out won't work) on Netscape Communicator and IE 5 Mac. At one point this was intentional but now its just worth mentioning.

Miscellaneous Files
-------------------

*font-stack.rtf* is a rich-text file for comparing the font stacks. Requires all the fonts in the stack to be loaded on a computer to actually compare them.

*test.html* is an example XHTML document delineating the variety of elements that the stylesheet affects for a simple visual reference. 

Example Definition To Be Placed In the `<head>` of an HTML Document
-------------------------------------------------------------------

`<!-- stylesheets -->
<link rel="stylesheet" type="text/css" media="screen" href="stylesheets/layout.css" />
<link rel="stylesheet" type="text/css" media="print" href="stylesheets/print.css" />

<!--[if lte IE 6]>
	<style type="text/css" media="screen">
		@import "stylesheets/ie6.css";
	</style>
<![endif]-->`