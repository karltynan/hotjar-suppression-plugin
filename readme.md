# Hotjar Suppression Bookmarklet

## What is it?

**Hotjar Suppression Bookmarklet** is a simple bookmarklet for your browser.

It highlights fields and markup on a page that are intended to be _suppressed_ when running *Hotjar* or *inspectlet* on your website.

## Installation

Just drag the following link to your bookmarks: 

<a href="javascript: (function () { e = document.createElement('LINK'); e.href = 'https://rawgithub.com/karltynan/hotjar-suppression-plugin/master/hotjar.css'; e.rel = 'stylesheet'; e.media = 'all'; document.body.appendChild(e); })();">
	<img src="assets/btn-drag.png" alt="Hotjar Suppression Test" />
</a>

Then visit a URL to test and press the bookmark to run the bookmarklet... Simple!

## Why?

I have created this bookmarklet as a response to GDPR when using Hotjar on websites.

If you are using *Hotjar* or *inspectlet*, you could be capturing secure or private information.

### Hotjar

The data attribute Hotjar provides, <code>data-hj-suppress</code>, allows you to _suppress_ the information being sent to Hotjar.

#### Test Hotjar

<p data-hj-suppress>This line of text will highlight when the bookmarklet has run.</p>

### inspectlet

The classes inspectlet provides, <code>.inspectletIgnore</code> for inputs and <code>.inspectlet-sensitive</code> for sensitive information, allows you to _suppress_ the information being sent to inspectlet.

#### Test inspectlet

<p class="inspectlet-sensitive">This line of text will highlight when the bookmarklet has run.</p>