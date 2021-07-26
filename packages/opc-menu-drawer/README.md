# opc-menu-drawer Component 👋

![Version](https://img.shields.io/badge/version-0.0.1-blue.svg?cacheSeconds=2592000)
![Build Status](https://travis-ci.org/dwyl/esta.svg?branch=master)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/1-Platform/op-components/graphs/commit-activity)

A web component based on Lit Element for Red hat One Platform Side Drawer.

## Prerequisites

Red Hat official font must be imported.

```css
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Text&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display&display=swap');
```

## Usage

```html
<opc-menu-drawer headerTitle="Akhil Mohan">
  <span slot="avatar"> Pi </span>
  <button slot="menu">Log In</button>
  <button slot="menu">Log Out</button>
  <span slot="footer"> 2021 Red Hat </span>
</opc-menu-drawer>
```

```js
const links = [
  {
    title: 'BUILD in SERVICES',
    links: [
      { name: 'Blog#1', href: '#' },
      { name: 'Documentation#1', href: '#' },
    ],
  },
  {
    title: 'BUILD in SERVICES',
    links: [
      { name: 'Blog#2', href: '#' },
      { name: 'Documentation#1', href: '#' },
    ],
  },
];

document.querySelector('opc-menu-drawer').links = links;
```

## Slots

There are total 5 slots available in this component

- `Default slot`: Default slot will be component inside body of the drawer componenent.

- `header`: Container component that contains the header component.

- `avatar`: The avatar component on drawer header.

- `menu`: The menu button on expanding drawer header.

- `footer`: Footer component of the drawer body.

## Attributes

- `links`
  - Type: `Array`
  - Default value: [ ]

```js
document.querySelector("opc-menu-drawer").links = {
    title: "BUILD in SERVICES",
    links: [
      { name: "Blog#2", href: "#" },
      { name: "Documentation#1", href: "#" },
    ],
  },;
```

- `headerTitle`
  - Type: `String`
  - Default value: `''`

```html
  <opc-menu-drawer headerTitle="Akhil Mohan"></opc-menu-drawer isOpen>
```

- `isOpen`
  - Type: `Boolean`
  - Default value: `false`

```html
<opc-menu-drawer isOpen></opc-menu-drawer>
```

## Events

- opc-menu-drawer doesn't have any events.

# CSS Variables

| CSS Variable name                           | Value             |
| ------------------------------------------- | ----------------- |
| `--opc-menu-drawer__backdrop-color`         | #00000060         |
| `--opc-menu-drawer__btn-hover-color`        | #efefef           |
| `--opc-menu-drawer__z-index`                | 9                 |
| ` --opc-menu-drawer__width`                 | 260px             |
| `--opc-menu-drawer__top`                    | 0px               |
| `--opc-menu-drawer__right`                  | #000              |
| `--opc-menu-drawer__menu-padding`           | 8px 21px          |
| `--opc-menu-drawer__link-group-title-color` | #6a6e73           |
| `--opc-menu-drawer__transition--default`    | 120ms ease-in-out |

## Install

```sh
npm install
```

## Usage

### Install opc-menu-drawer

```sh
npm install --save @one-platform/opc-menu-drawer
```

### For VanillaJS

- Import component

```js
import '@one-platform/opc-menu-drawer/dist/opc-menu-drawer';
```

- Add component in html

```html
<opc-menu-drawer> </opc-menu-drawer>
```

### For Angular

- In your app.module include the `CUSTOM_ELEMENTS_SCHEMA` and import the component

```js
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';
import '@one-platform/opc-menu-drawer/dist/opc-menu-drawer';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent],
})
export class AppModule {}
```

- Add component in any component html template

```html
<opc-menu-drawer> </opc-menu-drawer>
```

### For React

- Import the component in App.js

```js
import '@one-platform/opc-menu-drawer/dist/opc-menu-drawer';
```

- Add component in any component html render

```html
<opc-menu-drawer> </opc-menu-drawer>
```

### Development server

- Run development server

```sh
npm run dev opc-menu-drawer
```

### Build

```sh
npm run build opc-menu-drawer
```

## Run tests

```sh
npm run test
```

## 🤝 Contributors

👤 **[akhilmhdh](https://github.com/akhilmhdh)**
