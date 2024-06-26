# UI Libraries

_"Which UI library is the best"_ stands among the most common questions from newcomers to Vue.js ecosystem. The answer isn't easy though, since there is no such thing as "the best" components library for Vue, due to many factors that should be considered. What you can look for instead is a solution optimal for your specific use case.

Most of the libraries covered in this chapter are based on either Material Design or Ant Design, or provide Vue integrations for some framework agnostic UI libraries, such as Bootstrap, Bulma or Uikit.

[Roundup: Vue.js Desktop Web App Component Libraries](https://alligator.io/vuejs/roundup-desktop-components)

## Summary (TLDR)

If you don't have time to read all of this and just need a quick answer:

* [Vuetify](ui-libraries.md#vuetify) - mobile and desktop ready, material design
* [Quasar](ui-libraries.md#quasar) - material design as well but with cross-platform capabilities
* [Quasar](ui-libraries.md#quasar) - full framework, option of Cordova or Capacitor for mobile builds
* [Ionic Vue](ui-libraries.md#ionic-vue) - cross-platform UI toolkit, uses Capacitor for native mobile
* [Element UI](ui-libraries.md#element-ui) - extensive, desktop oriented, widely popular in asia
* [iView](ui-libraries.md#iview)
* [BootstrapVue](ui-libraries.md#bootstrapvue) - Bootstrap based
* [Buefy](ui-libraries.md#buefy) - Bulma based
* [Tailwind](ui-libraries.md#tailwind-css)

## How to chose an optimal UI library

This section is supposed to contain the guidelines on how to decide which UI library to use.

Here are some topics that should be covered:

* do you really need an UI library?
* how do you plan to approach mobile version of your website or application
* are you fine with a library that doesn't provide comprehensive support and large community
* what components are crucial for your project
* how important is SEO for your project, do you plan to use server side rendering?
* accessibility

## Material Design

Material Design is a very popular design concept not only in Vue.js world. Combining flat visual style with shadows and other lightning effects, it was primarily created with Android mobile applications in mind, but is widely used on traditional websites too.

The components in libraries such as [Vuetify](ui-libraries.md#vuetify) or [Vue-Material](ui-libraries.md#vue-material) look good by default, but since they were written with a certain design style in mind, they're not fully customizable. However, the new Material Design 2 specification brought more focus on flexible theming and we can expect the libraries to follow this move in 2019.

* [Material Design documentation](https://material.io/)

### Vuetify

> Vuetify is a semantic component framework for Vue. It aims to provide clean, semantic and reusable components that make building your application a breeze. Build amazing applications with the power of Vue, Material Design and a massive library of beautifully crafted components and features.

Vuetify is praised not only for a wide selection of components, but also for the way it's maintained. Currently it's developed by a full team of developers and it's got a big and well organized community. The project is funded via Patreon and Open Collective.

The library's ecosystem provides multiple tools, such as theme generator, Webpack loader or opinionated Eslint config. It's also easy to implement Vuetify in your application thanks to provided plugins for Vue CLI and Nuxt.

Internally, Vuetify is written with Typescript. The upcoming release of Vuetify 2 with improved theme system, accessibility and performance, will also bring the move from Stylus to SASS.

* [Vuetify repository](https://github.com/vuetifyjs/vuetify)
* [Vuetify documentation](https://vuetifyjs.com/en/)
* [Vuetify chat on Discord](https://community.vuetifyjs.com/)

### Quasar

> A massive pool of quality components ready for dropping directly into your existing or new projects today. Plus an easy to use build process, fully configurable (although 99% of the time you won't even need to touch it)... following all of the latest and greatest best web practices. Jumpstart a SPA, PWA, SSR, Mobile App or Desktop app in 30 seconds... (yes, it's that easy to get started!)

Quasar's emphasis is on a great developer experience. It offers its own CLI, which helps users with building applications for multiple platforms, including mobile apps via Cordova, desktop apps via Electron and PWAs or SPAs with or without Server Side Rendering (SSR). It has a growing community and a great team of developers, who are contributing a lot of time towards the project.

One of the features that sets Quasar apart from practically all other frameworks is its Application Extension System (or AE for short), where devlopers can not only use AE system for importing general code for their own projects, but can also share that same code with the general Quasar community. It's a powerful system, which allows Quasar projects to be extended with any number of different additions like with other components, additions of CLI commands and even application features. One great example is QCalendar - an intricate component for creating calendars.

* [Quasar repositories](https://github.com/quasarframework)
* [Quasar documentation](https://quasar.dev)
* [The QCalendar Component](https://github.com/quasarframework/app-extension-qcalendar)
* [List of Availabe App Extensions](https://quasar.dev/app-extensions/discover)
* [Quasar chat on Discord](https://chat.quasar.dev)
* [Forum](https://forum.quasar.dev)

### Vue Material

> Simple, lightweight and built exactly according to the Google Material Design specs.

The difference in popularity is big, but if you're looking for a library that follows Material Design principles to the letter, give it a try.

* [Vue Material repository](https://github.com/vuematerial/vue-material)
* [Vue Material documentation](https://vuematerial.io/)
* [Vue Material chat on Discord](https://discord.gg/vuematerial)

## Ant Design

Ant Design is kind of the opposite of previously mentioned Material Design. The libraries following this specification are meant to be used primarily on desktop, so their responsive design support is scarce.

The reason? Just like Material Design was created by Google, AntD is brought by designers from Alibaba - the largest e-commerce company in China. It's specifically targeted towards the Chinese web market, where traditional websites aren't usually accessed on mobile devices. Such libraries often provide separate solutions for mobile applications, based on a separate And Design Mobile specification.

This also means that they are maintained mainly by Chinese developers and it may be more difficult to get help in English.

Other than standard websites, Ant Design is a good choice for developers writing all kinds of administration systems.

* [Ant Design documentation](https://ant.design/)
* [Ant Design Vue](https://vuecomponent.github.io/ant-design-vue/docs/vue/introduce/)

### Element UI

In the worldwide context, Element UI is the most popular UI library for Vue.js and one of the oldest in the ecosystem. It also comes with a mobile sibling - Mint UI that can be used to write a hybrid application. It's got proper English documentation and a secondary international chat, but most of the Github issues are in Chinese.

Element UI provides starter kits for both general usage and Laravel projects, as well as Typescript bindings. There's a rich choice of components available and they can be imported on demand. The styles are written using SCSS with BEM methodology.

The library's success resulted in porting Element UI to Angular and React ecosystems.

* [Element UI repository](https://github.com/ElemeFE/element)
* [Element UI documentation](https://element.eleme.io/)
* [Element UI chat on Gitter](https://gitter.im/element-en/Lobby)

### iView

While not as well-known as Element UI, iView is a valid, well maintained alternative. It provides a large set of components which we can import on demand and useful tools to make working with them easier, together with Typescript support and the official admin panel template. It's a good choice especially if you prefer to work with LESS over SASS.

* [iView repository](https://github.com/iview/iview)
* [iView documentation](https://iviewui.com)

## Component sets for CSS Frameworks

Third group of UI libraries includes those that provide sets of components for traditional CSS frameworks. Both those which originally contain Javascript features, such as Bootstrap, Semantic UI or UIKit, and the purely CSS ones like Bulma. It's a good option if you're looking for some specific design style, you're already familiar with the CSS framework or you want to rewrite an already existing application that uses one of them.

Remember that you will still have to reach out to original framework's documentation and community for help, especially with styling.

### BootstrapVue

> BootstrapVue provides one of the most comprehensive implementations of Bootstrap V4.3 components and grid system available for Vue.js 2.6+, complete with extensive and automated WAI-ARIA accessibility markup.

If you want to use Bootstrap 4 for your project, BootstrapVue is the community's most often recommendation. It's a set of components natively written with Vue.js, so you don't have to worry about mixing Vue with JQuery. It's easy to use it with both Vue CLI and Nuxt.

BootstrapVue also includes several custom components based on Bootstrap v4 styling.

* [Bootstrap-Vue repository](https://github.com/bootstrap-vue/bootstrap-vue)
* [Bootstrap-Vue documentation](https://bootstrap-vue.org/)
* [Bootstrap-Vue chat on Discord](https://discordapp.com/invite/j2Mtcny)

### Buefy

Bulma grew up to be one of top CSS frameworks, but unlike most of them, it doesn't offer any Javascript functionality. That's where Buefy comes into play. It provides both a set of components and an easy way to integrate Bulma into your project.

Buefy's versions are synchronized with Bulma, so you can be sure that same versions of both frameworks are fully compatible with each other.

* [Buefy repository](https://github.com/buefy/buefy)
* [Buefy documentation](https://buefy.org/)
* [Buefy chat on Discord](https://discordapp.com/invite/ZkdFJMr)

### Vuikit

Vuikit is a Vue integration library that provides wrappers for [Uikit](https://getuikit.com/) framework. While not as well-known in Vue.js ecosystem as Bootstrap or Bulma, Uikit is a robust library that covers a wide variety of CSS & JS components, with some unique features that you won't find elsewhere out of the box.

* [Vuikit repository](https://github.com/vuikit/vuikit)
* [Vuikit documentation](https://vuikit.js.org/)
* [UIkit chat on Gitter](https://gitter.im/uikit/uikit)

### Semantic-UI-Vue

Despite its popularity, [Semantic UI](https://semantic-ui.com/) never really hit it off in Vue.js ecosystem. There were a few projects trying to bring good integration with Vue though. Out of them, the most noteworthy is Semantic-UI-Vue, inspired by a similar project from the React ecosystem.

* [Semantic-UI-Vue repository](https://github.com/Semantic-UI-Vue/Semantic-UI-Vue)
* [Semantic-UI-Vue documentation](https://semantic-ui-vue.github.io)
* [Semantic-UI-Vue chat on Gitter](https://gitter.im/Semantic-UI-Vue)

### Vectre

[Specter.CSS](https://picturepan2.github.io/spectre/) is a lightweight, responsive and modern CSS framework for faster and extensible development. The hallmark of this framework is its tiny size and consistent design language. But up to this point, there has been no full implementation of most of the components in any ecosystem. This was the motivation to create a fast, small and user friendly Vectre framework that will have modern features like typescript/tsx support, tree shaking, multiple JavaScript module systems and of course tiny size.

* [vectre repository](https://github.com/vectrejs/vectre)
* [vectre documentation](https://vectrejs.github.io/docs/)
* [vectre chat on Discord](https://discord.gg/4YTfpB)

### PrimeVue

[PrimeVue](https://www.primefaces.org/primevue/showcase/) is an advanced UI component library for Vue featuring 60+ rich set of components, a theme designer, various theme alternatives such as Material, Bootstrap, FluentUI, VueCLI templates and professional support. All widgets are open source and free to use under MIT License.

PrimeVue is developed by [PrimeTek Informatics](https://www.primetek.com.tr), a vendor with years of expertise in developing open source UI solutions including PrimeFaces, PrimeNG and PrimeReact

* [PrimeVue repository](https://github.com/primefaces/primevue)
* [PrimeVue documentation](https://www.primefaces.org/primevue/showcase/)

### Kendo UI for Vue

[Kendo UI for Vue](https://www.telerik.com/kendo-vue-ui) is a professionally built commercial UI library with 90+ components that is built for business applications. It provides [high-quality learning resources](https://www.telerik.com/kendo-vue-ui/components/) and an [award-winning technical support](https://www.telerik.com/best-tech-support). The components are fully responsive and accessible with support for multiple design systems like Kendo Default, Material Design, Bootstrap and the ability to create a custom variety of theme in [Theme Builder](https://themebuilder.telerik.com/kendo-vue-ui).

In [Telerik](https://www.telerik.com/) we've been solving this problem for the past 18 years across many development platforms, which now include four JavaScript frameworks.

* [Kendo UI for Vue repository](https://github.com/telerik/kendo-vue)
* [Kendo UI for Vue documentation](https://www.telerik.com/kendo-vue-ui/components/)

## Other solutions

### Tailwind CSS

> A utility-first CSS framework for rapidly building custom user interfaces.

Tailwind is very well accepted in the Vue community as it integrates very nicely with the concept of components. Integration is as simple as installing Tailwind and creating a config and importing it in your app.

* [Tailwind Docs](https://tailwindcss.com/docs/what-is-tailwind/)
* [Using Tailwind with Vue.js](https://flaviocopes.com/vue-tailwind/)
* [How to use Tailwind CSS in Vue together with CSS Modules](https://stefanzweifel.io/posts/how-to-use-tailwind-css-in-vue-together-with-css-modules)

### VueSax

The goal of VueSax is to provide an UI library focused on core JS functionality. While it offers a default design based on warm color palette, doesn't depend on any specific design language or CSS framework and by default uses native CSS variables rather than preprocessors.

Despite being less known than its mainstream competitors, VueSax has a track of consistent maintainment and managed to get a reputation of a stable UI solution.

* [VueSax repository](https://github.com/lusaxweb/vuesax)
* [VueSax documentation](https://lusaxweb.github.io/vuesax/)
* [VueSax chat on Discord](https://discord.gg/9dsKtvB)

### Inkline

> Inkline is a modern UI/UX Framework for Vue.js designed for creating flawless responsive web applications.

Inkline provides you with over 50 customizable components, hundreds of utility classes, and built-in schema-based Form Validation. The framework has been chosen as a finalist for the Open Source Awards at Vue.js London 2019, in the Developer Experience category.

* [Inkline repository](https://github.com/inkline/inkline)
* [Inkline documentation](https://inkline.io/)
* [Inkline chat on Discord](https://discord.gg/2w5UGnK)

### Ionic Vue

> A native Vue version of Ionic Framework that makes it easy to build apps for iOS, Android, and the web as a Progressive Web App. Our components allow developers to build native experiences, all while using web technology.

Ionic is an open source UI toolkit focused on building high quality cross platform apps. Originally built for Angular and already one of the most popular frameworks in the world, the latest release now supports Vue 3 as well as React thanks to their [move to native web components](https://blog.ionicframework.com/introducing-ionic-4-ionic-for-everyone) in version 4. The Ionic team reports the framework powers roughly [15% of all mobile apps](https://appfigures.com/top-sdks/development/apps).

* [Ionic Vue components](https://ionicframework.com/docs/components)
* [Ionic Vue documentation](https://ionicframework.com/docs/vue/overview)
* [Ionic Vue forum](https://forum.ionicframework.com/c/ionic/vue/29)
* [Your First Ionic Vue App](https://ionicframework.com/blog/new-tutorial-your-first-ionic-vue-app)

### Vuetensils

> A "naked" component library for building accessible, lightweight, on-brand applications.

Rather than a full-fledged framework, Vuetensils offers a set of base components that you can use to create your own UI system. It takes care of the raw JS functionality and accessibility, with only a minimal amount of default styling.

* [Vuetensils repository](https://github.com/stegosource/vuetensils)
* [Vuetensils documentation](https://vuetensils.stegosource.com)

### Chakra UI

Chakra is a Vue version of a popular UI library for React, with focus on accessibility. It makes use of [Styled System](https://styled-system.com/) which allows to declare CSS style properties directly via props, with a constrained set of utility classes.

While it depends on CSS-in-JS under the hood, you don't need to know it in order to use the library.

* [Chakra UI repository](https://github.com/chakra-ui/chakra-ui-vue)
* [Chakra UI documentation](https://vue.chakra-ui.com/)
