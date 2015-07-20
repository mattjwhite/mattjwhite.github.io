---
layout: post
title: "Route-Driven Security in Ember"
permalink: /route-sec/
---

One benefit of working with Ember is that it is straightforward to map standard presentation layer access control concepts to the Ember object model. For example, you might want only users with a certain role to visit certain locations. This maps nicely to Ember's use of routes.

Consider an app with an admin section. Clearly you don't want this admin UI visible to just anyone. And while your app might be diligent about locking down the UI around the admin route so you can't navigate to it via a link, your user can still try to alter the URL and browse directly to some variation on /admin.

 

Keep mind that presentation layer security is necessary, but nowhere near sufficient to secure your app. Much more is required of your server-side code for your app to be secure. However, by securing your presentation layer, you're accomplishing an important goal of security: usability.