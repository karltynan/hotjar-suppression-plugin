# Hotjar Suppression Bookmarklet

## What is it?

**Hotjar Suppression Bookmarklet** is a simple bookmarklet for your browser. It highlights fields and markup on a page that are intended to be _suppressed_ when running Hotjar on your website.

## Installation

Just drag the following link to your bookmarks: 

<a href="javascript: (function () { e = document.createElement('LINK'); e.href = 'https://rawgithub.com/karltynan/hotjar-suppression-plugin/master/hotjar.css'; e.rel = 'stylesheet'; e.media = 'all'; document.body.appendChild(e); })();">
	<img src="assets/btn-drag.png" alt="Hotjar Suppression Test" />
</a>

Then visit a URL to test and press the bookmark to run the bookmarklet... Simple!

## Why?

I have created this bookmarklet as a response to GDPR when using Hotjar on websites.

If you are using Hotjar, you could be capturing secure or private information.

The data attributes Hotjar provides, such as <code>data-hj-suppress</code>, allow you to _suppress_ the information by sending asterisks "***" or 1s "111" for each character instead.

## Test it!

<p data-hj-suppress>This line of text will highlight when the bookmarklet has run.</p>