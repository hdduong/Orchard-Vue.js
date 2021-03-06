# Vue.js module for Orchard Core



## Project description

[Orchard Core](http://orchardproject.net/) module that contains [Vue.js](https://vuejs.org/) and commonly used Vue.js components to be used in other Vue.js apps as dependencies. Provides extensibility to create Vue.js component templates as Orchard Core shapes making them able to override in themes or modules.


## Prerequisites

1. Make sure that you have the latest version of [Node.js](https://nodejs.org/en/) installed that fits your system architecture (x64 or x86).
2. Install or update NPM to the latest version using the command: `npm install -g npm@latest`
3. Install or update the Gulp CLI globally with this command: `npm install -g gulp-cli`


## Using Vue.js node packages

The packages will be automatically installed on build (i.e. `dotnet build`) or you can trigger it using the `npm install` command.


## Adding Vue.js component templates

Place your template files (.cshtml or .liquid) to the *Views/VueComponents* folder. The shape template harvester will harvest these templates and the generated shape type will be as it would be normally generated but with `VueComponent-` prefix. Eg.:

    <shape type="VueComponent-App_UserProfile"></shape>

In these shapes you can use any format you want (e.g. JSX templates) and reference their id in your Vue.js component JavaScript code.


## Other resources

Some resources are registered in the resource manifest so you can add these as dependencies to your Vue.js app's resource. These resources are automatically copied from the *node_modules* folder to *wwwroot* using Gulp when building the project (or you can trigger it with the `gulp` command).

- [ES6-Promise](https://www.npmjs.com/package/es6-promise): Use this if you want to use ES6 Promises (or an ES6 module that uses them e.g. `axios`) include this resource so it will work in IE as well.


## Contribution and feedback

The module's source is available in two public source repositories, automatically mirrored in both directions with [Git-hg Mirror](https://githgmirror.com):

- [https://bitbucket.org/Lombiq/orchard-vue.js](https://bitbucket.org/Lombiq/orchard-vue.js) (Mercurial repository)
- [https://github.com/Lombiq/Orchard-Vue.js](https://github.com/Lombiq/Orchard-Vue.js) (Git repository)

Bug reports, feature requests and comments are warmly welcome, **please do so via GitHub**. Feel free to send pull requests too, no matter which source repository you choose for this purpose.

This project is developed by [Lombiq Technologies Ltd](https://lombiq.com/). Commercial-grade support is available through Lombiq.