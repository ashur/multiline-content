---
title: Importing external components in WebC via NPM
draft: true
---
<mc-aside>
  This post assumes familiarity with Eleventy, a static-site generator. (You know the one; it's basically all I ever write about here). 
</mc-aside>

I finally started playing around with WebC, and I think a relatively small feature — webc:import — will make it an especially compelling choice for building components that can be easily shared between Eleventy projects.

## What is WebC

![Code snippet showing a WebC component named "ac-button" that is imported from an external NPM package](https://user-images.githubusercontent.com/3238096/209586839-18254e6e-da5e-418f-b324-52c7e1b14914.png)

WebC is a new tool that adds first-class component support to Eleventy without all the client-side JavaScript that commonly bloats sites built with similar tools. (Even cooler, it's framework-agnostic!)

I've only scratched the surface of what WebC can do, but I already see there's a lot to like:

- Support for Vue-like single-file component definitions — component HTML, CSS, and JavaScript all in one file
- Optionally scoped CSS, adding a prefix class to help prevent selector collisions across styles
- Asynchronous support across the board!

These tentpole features sound like a first-rate foundation for building reusable components, but one small note in the docs has me just as excited:

> New in WebC v0.6.2, you can import directly from an installed npm package.

_Go on..._
