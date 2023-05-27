# *Content Substitution Plan*

###### last edit: 23-01-12

## Tasks
1. make search work
   - see documentation
2. replace content for ~20 pages generated from markdown files
   - change en-us
   - change other NL MD pages for target page
   - test search
3. change sidebar menu items for #2
   - update _blueprint.yaml
4. change font source
   - https://github.com/ampproject/amp.dev/tree/a6817519c19987b8a700110e9909f3c3bafce769/boilerplate/templates/partials/fonts
5. change main menu page
   - https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/about
   - https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/about/_blueprint.yaml
6. change SVG for main menu

## Contributing content instructions
- https://github.com/ampproject/amp.dev/blob/future/contributing/documentation.md
- https://github.com/ampproject/amp.dev/blob/future/contributing/samples.md


## URL title set here
```
$title: AMP - a web component framework to easily create user-first web experiences
```
-  need to replace with 20 digit IDN
- find NL version
- reset in <head>

## ampproject/amp.dev

### BRANCH: future

- find the switch betwewn CSS used for front pages and CSS used for sidebar pages
   - default.j2
   - css/components/templates/default.css
- vs
   - custom.j2
   - /css/components/templates/component-overview.css

## The official homepage of the AMP Project.

### about: The AMP Project Website
- https://github.com/ampproject/amp.dev/
- https://github.com/ampproject/amp.dev/tree/future/
- https://github.com/ampproject/amp.dev/tree/future/pages/
- https://github.com/ampproject/amp.dev/tree/future/pages/content/
- https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/

### homepage for all projects; no sidebar
- https://amp.dev/
   - text: The latest news
   - https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/index-2021.html

### issue: where is this page
- https://amp.dev/fr/index-2021/

#### Website
- https://amp.dev/about/websites/
- https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/about/websites-2021.html

### list menus-main
- https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/about/_blueprint.yaml

### inject SVG for menus-main
- https://github.com/ampproject/amp.dev/blob/a6817519c19987b8a700110e9909f3c3bafce769/frontend/templates/views/2021/partials/header.j2

```
$title@: About
$path: /about/{base}.html
$view: /views/default.j2
$localization:
  path: /{locale}/about/{base}.html
```
FR page
- https://amp.dev/fr/about/websites-2021/
- https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/documentation/

### partials
- https://github.com/ampproject/amp.dev/tree/a6817519c19987b8a700110e9909f3c3bafce769/frontend/templates/views/partials

### intermediate page avec cards; includes sidebar
- /views/partials/sidebar-toggle-button.j2
- https://github.com/ampproject/amp.dev/tree/a6817519c19987b8a700110e9909f3c3bafce769/frontend/templates/views
- https://github.com/ampproject/amp.dev/blob/a6817519c19987b8a700110e9909f3c3bafce769/frontend/templates/views/partials/sidebar-toggle-button.j2
- https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/documentation/components/
- https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/documentation/components/index.html
- https://amp.dev/documentation/components/
- https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/documentation/components/index.html
- https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/documentation/components/reference

### NL page list

## ampproject/amphtml

### where source code is stored

#### has documentation parallel to amp.dev

- BRANCH: main
- about: The AMP web component framework
https://github.com/ampproject/amphtml/
https://github.com/ampproject/amphtml/tree/main/
https://github.com/ampproject/amphtml/tree/main/extensions
   - list of items in sidebar

https://amp.dev/documentation/components/amp-list/
https://github.com/ampproject/amphtml/blob/main/extensions/amp-list/
https://github.com/ampproject/amphtml/blob/main/extensions/amp-list/amp-list.md

https://amp.dev/documentation/components/amp-autocomplete/
https://github.com/ampproject/amphtml/tree/main/extensions/amp-autocomplete
https://github.com/ampproject/amphtml/blob/main/extensions/amp-autocomplete/amp-autocomplete.md
