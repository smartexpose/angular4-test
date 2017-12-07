# Frontend Angular 4 Test

This project was generated with [angular-cli](https://github.com/angular/angular-cli)

- version 1.0.0-beta.28.3.
- dependencies updated to Angular `v4.0.0`

## Installation

- clone project
```
$ git clone https://github.com/smartexpose/angular4-test.git
```

- install dependencies
```
$ cd angular4-test
$ npm install
```


## Run the app
```
$ npm start
```

- Navigate to `http://localhost:4200/`. 
- The app will automatically reload if you change any of the source files.

## Generating new components, services, pipes, etc

- Run `ng generate component component-name` to generate a new component.
- For more detailed instructions, see `https://github.com/angular/angular-cli`

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
   - Shared service which provides a simple method to load the data, i.e., array of entries (title, image, text) asynchronously with RxJs Observables.

**Pipes**

- `FirstUppercasePipe`:
   - A simple pipe that capitalizes the first letter of a word
   - It should be used to capitalize the `title` and `text` fields in each `<blog-entry>`
