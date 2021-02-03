---
title: "Progressive Web Apps"
seo_title: "Building Progressive Web Applications in Mendix - Responsive Design"
seo_description: "Learn how Mendix progressive web apps work & how Mendix's responsive design means applications will look great no matter which resolution or device they're displayed on."
parent: "ux-multi-channel-apps"
menu_order: 50
bg: "ux"
tags: ["web app", "app", "pwa", "progressive", "application"]
---

## 1 How Do Mendix Progressive Web Apps (PWA) Work?

A progressive web app (PWA) is a special type of web application that progressively uses more functionality from the browser to improve the user experience. Mendix progressive web apps are similar to [web applications](web-apps), but PWAs offer more functionality — such as an option to work partially or fully offline, an option to be added to the device's home screen, and support for device capabilities and web push notifications. PWAs are often used for mobile apps, but they can also be used for desktop apps.

Developers can create a PWA similar to how they create a web app. This symmetry gives developers all the options they are used to, and enables them to re-use existing components and knowledge. In addition, developers can apply an [offline-first](offline-apps) approach to improve the performance and availability of their app.

Developers can enable just the PWA features their use case requires, for example **Add to Home Screen** support, resource caching (for things like pages, styling, and logic), or full offline support. Developers can also add functionality to leverage device functionality like the camera, location services, or add support for web push notifications. Note that the available features depend on browser capabilities.

As discussed in the [How Does Mendix Support Multi-Channel Applications?](front-end#support-multi-channel) section of *Front-End*, a PWA is one possible channel for Mendix applications. The Mendix Client is responsible for rendering web apps, which are rich single-page applications (SPA) based on JavaScript, HTML5, and CSS3. PWAs also use service workers to cache data and improve performance.

Using the WYSIWYG page editor in Mendix Studio and Mendix Studio Pro, users can model pages and interactions that can run locally or be deployed directly from Mendix Studio and Mendix Studio Pro. When running locally, the changes are made visible directly. This is done with our **instant update** feature that instantly reloads the UI while preserving the current state, making testing and previewing apps a breeze.

When an app is deployed to the cloud, the static resources (HTML, CSS, JavaScript) are deployed on a front-facing server that caches and efficiently serves the resources. PWAs can also cache the resources in the user's browser for improved performance. The main entry is the *index.html* page, which loads the Mendix Client, renders the page, and starts handling events. If authentication is needed, the end-user is redirected to either the login page or an identity provider. Mendix makes sure that there are no caching issues when deploying new versions by applying a cache-busting mechanism.

The Mendix JavaScript Client renders the UI, handles actions in the browser, and communicates through APIs via HTTPS with the Mendix Runtime. This rich client can perform many actions without the need to call the server, thus minimizing the number of costly server round-trips. Combined with our [client-side functionality](front-end#support-client-side-logic) and the fact that Mendix apps support browsers' back/forward functionality while complying with accessibility guidelines, you can efficiently model web apps with excellent performance.

## 2 How Does Mendix Support Different Screen Sizes & Devices?

Mendix pages are responsive by default, so they automatically adjust to screen size. This results in web apps that look great out of the box on screen sizes ranging from desktops to phones. For an optimized user experience, you can define separate mobile web channels for phone and tablet. The device type (as in phone, tablet, or desktop) can also be used in the logic for other scenarios.

<video controls src="attachments/Eval_Mobile_ResponsiveFormFactorsBuild_V2-2.mp4">VIDEO</video>

Mendix provides several common patterns and best practices per device to help you build great user experiences. You can also extend these patterns with custom variants, as discussed in [User Interface Design](ui-design).

## 3 How Can I Extend My Progressive Web App?

Mendix offers several options for extending web apps. These are discussed in the section [How Can I Extend the Mendix Front-End?](front-end#extend) of *Front-End* and the section [How Can I Customize the Look and Feel of My Apps?](ui-design#customize) of *User Interface Design*.

Based on settings a default [Web App Manifest](https://www.w3.org/TR/appmanifest/) is generated, but developer can fully customize if needed. Next to that, both the *index.html* and login page can be fully customized to your needs. 

## 4 How Can I Test or Distribute My Progressive Web App?

As PWAs are web apps, these can be easily tested and distributed by opening the URL in a browser. For local development, Mendix generates a QR code so you can quickly test a PWA on a mobile device.

## 5 How Can I Test My Progressive Web App?

Mendix offers an integrated [Application Testing Suite (ATS)](https://docs.mendix.com/ats/), in which (non-technical) users can test web applications using recorded test scripts on multiple browsers and multiple devices.

{{% image_container width="600" %}}
![Application Testing Suite](attachments/ats.png)
{{% /image_container %}}

It is also possible to use standard test tooling, like [Selenium](https://www.seleniumhq.org/). Because Mendix widgets have unique identifiers in the document object model (DOM), test tooling can easily leverage these IDs to create readable and robust test scripts.
