+++ 
draft = false
date = 2021-02-01T10:58:11+05:30
title = "Simple tips to Optimize Web Site Performance"
slug = "" 
tags = [""]
categories = [""]
description = "Simple and short tips"
+++

### Using CSS Sprites and reduce resource fetches in a website

Ever noticed you do multiple fetches to get lots of icons and your site has to wait for all fetches to complete therefore increasing site startup time.

To solve this images/icons are packed into a sprite sheet to reduce the number of image resources that need to be fetched in order to display a page.

For more technical details [Click Here](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Images/Implementing_image_sprites_in_CSS).

### Using HTTP2 (HTTPS) over plaintext HTTP

HTTP2 uses a binary payload over the HTTP plaintext payload binary is faster for the browser to parser therefore faster for the browser to render

### Using a compression algorithm to compress assets sent over HTTP

This is usually a web server configuration most web servers do this by default if configured properly.
Compression algorithms consists of gzip , bzip2 ,brotli with brotli being the best. 
Chrome doesn't allow brotli over HTTP 1.1 or lower therefore making switching to HTTP2 an ideal solution.