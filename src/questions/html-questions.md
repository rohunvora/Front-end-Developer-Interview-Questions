---
title: HTML Questions
layout: layouts/page.njk
permalink: /questions/html-questions/index.html
---

* What does a `doctype` do?
It just makes sure that your HTML doc will work on any browser.
* How do you serve a page with content in multiple languages?
``` HTML text/html; charset=utf-8 or application/x-www-form-urlencoded; charset=utf-8) ```
* What kind of things must you be wary of when designing or developing for multilingual sites?
* What are `data-` attributes good for?
Allows you to store information in the tag without displaying it on the main page.
* Consider HTML5 as an open web platform. What are the building blocks of HTML5?
Text Markup
Form Elements
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
``cookies`` only allow you to store strings.
``sessionStorage`` and localStorage allow you to store JavaScript primitives but not Objects or Arrays.
``Session storage`` will generally allow you to store any primitives or objects supported by your Server Side language/framework.
* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
script: loads a client-side script
script-async: the page load will not be dependent on this script, so it will continue to load as the overall page is loading
script defer: only run this script once the page is done loading.

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
It needs to check the CSS before it loads the body, but doesn't need it to load the head since nothing in head is displayed on the page.
* What is progressive rendering?
A technique to load content where it starts low quality and then becomes higher quality as more of the page loads.
* Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute.
This is so if you have different sizes of the same image, you can set multiple images to the same src tag so at different browser sizes, you can display a different size image.
* Have you used different HTML templating languages before?
Yes, EJS.
* What is the difference between `canvas` and `svg`?
SVG gives better performance with smaller number of objects or larger surface. Canvas gives better performance with smaller surface or larger number of objects.
