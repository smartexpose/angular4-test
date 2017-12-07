# Angular4Test

This project was generated with [angular-cli](https://github.com/angular/angular-cli) version 1.0.0-beta.28.3.

## Development server
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive/pipe/service/class/module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Deploying to GitHub Pages

Run `ng github-pages:deploy` to deploy to GitHub Pages.

## Further help

To get more help on the `angular-cli` use `ng help` or go check out the [Angular-CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

<hr>

## Test description

### **Goals and priority:**
- Create a very basic _single-page_ blog for Angular news
- Demonstrate practical understanding of Angular 2+, core concepts and implementation.

### **Starting material:**
- `screenshots/**`: images illustrating the expected page contents
- `data/entries.ts`: first 2 entries for the blog
- dfeault _angular-cli_ core working project including
   - `app.module.ts`
   - `app.component.ts`

### **What you must generate:**

**Templates (html)**

The following contents must be shown from top to bottom:

- `<h2>` header with text: 'Angular Blog'
- List of `<blog-entry>` elements which can dynamically grow
- `<form>` where the user can add a new Blog entry

**Models**

- `BlogEntry`:
  - A simple interface for handling the 3 fields (title, image, text)
  contained in each blog entry

**Components**

- `BlogComponent`
   - This is the main presentation Component which contains the template
   - The component's selector `blog` should be included in the _app.component.html_

- `BlogEntryComponent`
   - This component displays each blog entry, namely:
      - title
      - image (url)
      - text

**Services**

- `BlogService`:
   - Shared service which provides a simple method to load the data, i.e., array of entries (title, image, text) asynchronously

**Pipes**

- `FirstUppercasePipe`:
   - A simple pipe that capitalizes the first letter of a word
   - It should be used to capitalize the `title` and `text` fields in each `<blog-entry>`
