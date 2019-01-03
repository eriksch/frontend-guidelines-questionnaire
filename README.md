# Frontend Guidelines Questionnaire
---------------

## CSS 

### CSS Principles
- **What are some general principles your team should follow when writing CSS?** *(For example, modularity, avoiding long selector strings, etc. See [these](http://cssguidelin.es/) [resources](http://www.yellowshoe.com.au/standards/#css) [for](http://manuals.gravitydept.com/code/css) [inspiration](http://codeguide.co/#css))*

- Simple selectors
- CSS folder structure is as follows:

### CSS Methodology
- **Is your team using a CSS methodology** *(such as [SMACSS](https://smacss.com/), [BEM](https://en.bem.info/method/), or [OOCSS](http://oocss.org/))*? If yes, where is the documentation for that methodology?
- **Are you deviating from the methodology in any way?** If so, can you highlight these conventions?

- BEM where applicable (when control over html/css is possible).
- Avoid use of selector concatenation
- Namespace everything above atomic level.

### CSS Tools
- **Is the team using a preprocessor** *SCSS*?
- **Are you using a CSS base** *Reboot*?
- **Are you using any CSS postprocessors** *Autoprefixer - postcss*?
- **Are there specific CSS techniques you're utilizing** *Thinking about critical CSS*?

### CSS Frameworks
- **Is the team using a framework** *Minimal Bootstrap + Custom function*?
- **Are you deviating from the framework in any way?** *Just the bootstrap basics - Then everthing is organized using Brad Frosts Atomic design*

### CSS Style
- **Spaces or Tabs?** 
.editorconfig

[*.scss]
indent_style = space
indent_size = 4
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true


- **[Grouping] properties?** Flex and Grid properties via CSS linting

---------------

## JavaScript

### JavaScript Principles
- **What are some general principles your team should follow when writing JavaScript?** *drupal style when in a module*

### JavaScript tools
- **Are you using a JavaScript framework** *Jquery*?
- **Are you using any polyfills or shims** *Drupal has some defaults*?
- **What third-party scripts are dependencies for your project** *GSAP for complex animations - see package.json for other libs*?
- **Do you test your JavaScript?** *Not yet*

### JavaScript Style 
- **Spaces or Tabs?**
.editorconfig

[*.{js,twig}]
indent_style = space
indent_size = 2
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true

- **What patterns are you following?** *drupal module pattern*

---------------

## Media
- **How are you handling icons** *Preferred to use SVG when possible. Optimized to include in the body and reference where needed.*
- **How are you handling responsive images** *Drupal native*?
- **Are you using any tools to optimize and serve images** *Drupal native*?

---------------

## Fonts
- **How do you load custom fonts?** *@import*
- **Do you use any tools to help implement web fonts** *Font Squirrel*?

---------------

## Performance
- **Do you use performance budgets?** *budget for pageload is around 2 to 2.5 sec*
- **How are you measuring your project's speed** *Done by measureworks*?
- **What techniques are you using to decrease file size** *gzip*?
- **What performance-related tools are you using in your workflow?** *nothing yet*?


---------------

## Accessibility
- **Are you following the accessibility recommendations laid out in [this checklist](http://a11yproject.com/checklist.html)?** *We should*
- **What accessibility-related [tools](http://a11yproject.com/resources.html) are you using in your workflow?** *We should* 

---------------

## Tooling
- **Are you using a task runner** *webpack 4 build*?
- **Are you using a dependency manager** *Composer and Yarn*?
- **Are you using any scaffolding tools** *no*?
- **Are you using any tools to reinforce frontend style** *Editor Config and scsslint*?
- **Are any other specific pieces of software that are needed to work on this project?** *lando for local dev*
 
---------------

## Version control
- **What version control system are you using for your frontend code** *gitlab*?
- **Do you use a version control workflow** *feature-branch*?
- **Who's responsible for managing and governing the version controlled code?**? *the maintainers*
- **Where are issues tracked?** *Jira*

-----------

## Support and Optimization

- **What browsers are you *optimizing* for?** *IE 10 minimal and up*
- **What devices are you *optimizing* for?**  
- **Are you using a [graded browser support](https://github.com/yui/yui3/wiki/Graded-Browser-Support) system?**
- **Are there specific components that require [more specific grading](https://www.filamentgroup.com/lab/grade-the-components.html)?** 

-----------

## Localization
- **Is your website served in different languages?** *Yes*

-----------

## Deployment/Integration
- **How is your front-end code integrated into a production environment?** *gitlab CI pipeline* 


