# angular 5.0+ calendar

[![Build Status](https://travis-ci.org/mattlewis92/angular-calendar.svg?branch=master)](https://travis-ci.org/mattlewis92/angular-calendar)
[![codecov](https://codecov.io/gh/mattlewis92/angular-calendar/branch/master/graph/badge.svg)](https://codecov.io/gh/mattlewis92/angular-calendar)
[![npm version](https://badge.fury.io/js/angular-calendar.svg)](http://badge.fury.io/js/angular-calendar)
[![devDependency Status](https://david-dm.org/mattlewis92/angular-calendar/dev-status.svg)](https://david-dm.org/mattlewis92/angular-calendar?type=dev)
[![GitHub issues](https://img.shields.io/github/issues/mattlewis92/angular-calendar.svg)](https://github.com/mattlewis92/angular-calendar/issues)
[![GitHub stars](https://img.shields.io/github/stars/mattlewis92/angular-calendar.svg)](https://github.com/mattlewis92/angular-calendar/stargazers)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/mattlewis92/angular-calendar/master/LICENSE)

## Table of contents

- [About](#about)
- [Getting started](#getting-started)
- [Documentation](#documentation)
- [Breaking changes](#breaking-changes)
- [FAQ](#faq)
- [Angular 1 version](#angular-1-version)
- [Development](#development)
- [License](#license)

## About

A calendar component for Angular 5.0+ that can display events on a month, week or day view.

## Getting started

First install through npm:

```bash
npm install --save scheduler-calendar
```

Next include the CSS file somewhere into your app:

```
node_modules/scheduler-calendar/css/angular-calendar.css
```

Finally import the calendar module into your apps module:

```typescript
import { NgModule } from '@angular/core';
import { BrowserAnimationsModule } from '@angular/platform-browser/animations';
import { CalendarModule } from 'scheduler-calendar';

@NgModule({
  imports: [
    BrowserAnimationsModule,
    CalendarModule.forRoot()
  ]
})
export class MyModule {}
```

In order to allow the most flexibility for all users there is a substantial amount of boilerplate required to get up and running. Please see the [demos list](https://mattlewis92.github.io/angular-calendar/) for a series of comprehensive examples of how to use this library within your application. 

Once you are up and running, to access a full list of options for each component, the individual APIs are documented here: [`mwl-calendar-month-view`](https://mattlewis92.github.io/angular-calendar/docs/components/CalendarMonthViewComponent.html), [`mwl-calendar-week-view`](https://mattlewis92.github.io/angular-calendar/docs/components/CalendarWeekViewComponent.html) and [`mwl-calendar-day-view`](https://mattlewis92.github.io/angular-calendar/docs/components/CalendarDayViewComponent.html).

### Module bundlers

You can find quick start examples for all common module bundlers in the [build-tool-examples](https://github.com/mattlewis92/angular-calendar/tree/master/build-tool-examples) folder.

## Documentation

To see all available API options, take a look at the auto generated [documentation](https://mattlewis92.github.io/angular-calendar/docs/). You may find it helpful to view the examples on the demo page.

## Breaking changes

Where possible this library will strictly adhere to [semver](http://semver.org/) and only introduce API breaking changes in 0.x releases or new major versions post 1.0. The only exception to this is if you are using custom templates or extending the base components to add additional functionality, whereby critical bug fixes may introduce breakages as the internal API changes.

## Development

### Prepare your environment

* Install [Node.js](http://nodejs.org/) and NPM (should come with)
* Install local dev dependencies: `npm install` while current directory is this repo

### Development server

Run `npm start` to start a development server on port 8000 with auto reload + tests.

### Testing

Run `npm test` to run tests once or `npm run test:watch` to continually run tests.

### Build

* Bump the version in package.json (once the module hits 1.0 this will become automatic)

```bash
npm run build
```

## License

MIT
