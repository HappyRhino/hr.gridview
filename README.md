hr.gridview [![Build Status](https://travis-ci.org/HappyRhino/hr.gridview.png?branch=master)](https://travis-ci.org/HappyRhino/hr.gridview)
=============================

> Grid view for HappyRhino

## Installation

```
$ npm install hr.gridview
```

## Documentation

Create a new grid:

```js
var GridView = require("hr.gridview");

var grid = new GridView();
```

Append views:

```js
grid.addView(yourView);
grid.addView(yourSecondView);
```

Change layout by changing the number of columns:

```js
// Default is 0, for an auto grid layout
grid.setLayout(0);

// the 2 views will be side by side
grid.setLayout(2);

// the first view will be on top of the other
grid.setLayout(1);
```

Hide a view from the grid without removing it:

```js
yourView._gridOptions.enabled = false;
grid.update();
```
