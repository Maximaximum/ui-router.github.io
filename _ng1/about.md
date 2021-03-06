---
title: "UI-Router for Angular 1"
layout: single
excerpt: "The defacto standard for routing in AngularJS"
sitemap: true
permalink: /ng1/
---
{% include toc icon="columns" title="Angular 1" %}

<center>
<img src="/images/logos/angular1.png">
</center>

## About 

UI-Router is the defacto standard for routing in AngularJS.
Influenced by the core angular router `$route` and the Ember Router, 
UI-Router has become the standard choice for routing non-trivial apps in Angular 1.

## Getting UI-Router

The UI-Router package is distributed using [npm](https://www.npmjs.com/), the node package manager.

```
npm install --save angular-ui-router
```

Other examples:

- Via command line
  - Adding the latest prerelease to your project: `npm install --save angular-ui-router@next`
  - Adding a specific version to your project: `npm install --save angular-ui-router@1.0.0-beta.1`
  
- From <http://unpkg.com> via a `<script>` tag in your html: 
  - Latest stable version: `<script src="//unpkg.com/angular-ui-router/release/angular-ui-router.min.js">`
  - A specific version: `<script src="//unpkg.com/angular-ui-router@0.3.1/release/angular-ui-router.js">`
  
- From bower: `bower install angular-ui-router#0.3.1`

Note: bower releases are considered 'legacy' and are managed at <https://github.com/angular-ui/angular-ui-router-bower>
  
## Tutorials

Learn UI-Router by following our tutorials.

- [Hello World](/tutorial/ng1/helloworld)
- [Hello Solar System](/tutorial/ng1/hellosolarsystem)
- [Hello Galaxy](/tutorial/ng1/hellogalaxy)
 
 
## Sample application

The [UI-Router Sample App](/resources/sampleapp) is a non-trivial UI-Router application.
 
## Development

To fix a UI-Router bug, or create an enhancement, follow these steps: 

The Typescript source code for UI-Router for Angular 2 can be found at <https://github.com/angular-ui/ui-router>
UI-Router for Angular 1 depends on UI-Router Core, which can be found at <https://github.com/ui-router/core>

To get started:

```
git clone https://github.com/angular-ui/ui-router angular-ui-router
git clone https://github.com/ui-router/core ui-router-core
cd ui-router-core
npm install
npm link
npm run build

cd ../angular-ui-router
npm install
npm link ui-router-core
npm run build
```

To create a UI-Router bundle to test a bug fix against your app, run `npm run package`
You can then run `npm link`, and then run `npm link angular-ui-router` in your app's directory.
Your app's npm dependency will use the local `angular-ui-router` package that you just built. 

Alternatively, bundles are also created in `release/angular-ui-router.js`.


