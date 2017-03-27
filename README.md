
## 2017-03-27
A sheep teaching other sheep how to be a wolf

### What's new
- Auto generated changelogs
- Mono repos
- Storybook
- github pages
- Hyperion reference
- Artifactory
- "White label" theming

### Roc basics  
_Roc_ solves _JS fatigue_ and provides a better developer experionce (DX)
Read more http://www.getroc.org/, https://github.com/rocjs/roc, [documentation](https://github.com/rocjs/roc/blob/master/docs/README.md).

### Roc project components (packages, plugins, templates...)
> A little confusing to what is what and how it should be used. A little sparse documentation.

#### Roc extensions (packages & plugins)
Create a project using one or many Roc extension as a starting point. `npm i --save-dev <package>`
Essentially a predefined collection of _npm libraries_ with minimal and working configuration.

> The difference between a package and a plugin is not that big. Plugins are smaller and cannot be used
on its own, it adds capabitilites but has no "base". At least on package always needs to be included.

#### Roc template
Will help you set up a project through interactive _CLI_. `roc init <template>`
Essentially a wrapper to _Roc extensions_ with interaction.

### Artifactory
Not so open source. Needed for most new _Roc_ components.

Setup with variables to be able to use cross projects.

### Storybook
Minimal app to run/test/develop _React_ components.

### White label theming
New! All web components should use white label theming. Meaning; designed to always take a theme as input to the component.
Default theme included in the package, easilly overwritten. Sort of synced with _UX DNA_.

### Reflections building "Notifications"
> Truly stand-alone requires some thinking. Do we go full retard?
>
> API integrations a bit messy because of cross site scripting. We should either expose everything via a proxy or find a nice "local proxy" solution.
>
> Not having Redux is a context switch.
>
> Passing parameters to API needs maybe a standard (even if it is ours)
>
> Picking up data from cookies - is it really the best practice?

## 2017-03-23
- Reference implementation of a "hyperion" app; consuming web components  
  [/smp-distribution/hyperion-reference](https://github.schibsted.io/smp-distribution/hyperion-reference)
## 2017-03-21
- Reference implementation of a web component  
  [/smp-distribution/web-components/](https://github.schibsted.io/smp-distribution/web-components)
- A step-by-step guide to creating a stand-alone React component using roc-plugin-mono.  
  [/schibsted-martin/roc-notify/HOWTO.md](https://github.com/schibsted-martin/roc-notify/blob/master/HOWTO.md)
