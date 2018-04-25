# Hotjar Suppression Bookmarklet

## What is it?

**Hotjar Suppression Plugin** is a CSS bookmarklet for your browser. It highlights fields and markup on a page that are intended to be _suppressed_ when running Hotjar on your website.

## Installation

Just drag the following link to your bookmarks: 

<a href="javascript%3A%20(function%20()%20%7B%20e%20%3D%20document.createElement(%27LINK%27)%3B%20e.href%20%3D%20%27https%3A%2F%2Frawgithub.com%2Fkarltynan%2Fhotjar-suppression-plugin%2Fmaster%2Fhotjar.css%27%3B%20e.rel%20%3D%20%27stylesheet%27%3B%20e.media%20%3D%20%27all%27%3B%20document.body.appendChild(e)%3B%20%7D)()%3B">Hotjar Suppression Encoded</a>

<a href="javascript: (function () { e = document.createElement('LINK'); e.href = 'https://rawgithub.com/karltynan/hotjar-suppression-plugin/master/hotjar.css'; e.rel = 'stylesheet'; e.media = 'all'; document.body.appendChild(e); })();">Hotjar Suppression Unencoded</a>

Then visit a URL to test and press the bookmark to run the bookmarklet... Simple!

## Why?

I have created this as a requirement of GDPR. If you are using Hotjar, you will often be capturing secure or private information. The special data attributes Hotjar provides, such as <code>data-hj-suppress</code>, allow you to _suppress_ the information being recorded into "*"s or "1"s. This bookmarklet