# Hotjar Suppression Bookmarklet

## What is it?

**Hotjar Suppression Plugin** is a CSS bookmarklet for your browser. It highlights fields and markup on a page that are intended to be _suppressed_ when running Hotjar on your website.

## Installation

Just drag the following link to your bookmarks: 

<a href="javascript: (function () { e = document.createElement('LINK'); e.href = 'https://rawgithub.com/karltynan/hotjar-suppression-plugin/master/hotjar.css'; e.rel = 'stylesheet'; e.media = 'all'; document.body.appendChild(e); })();">Hotjar Suppression Bookmarklet</a>

Then visit a URL to test and press the bookmark to run the bookmarklet... Simple!

## Why?

I have created this as a requirement of GDPR. If you are using Hotjar, you will often be capturing secure or private information. The special data attributes Hotjar provides allow you to _suppress_ the information being recorded into "*"s or "1"s. This bookmarklet