# Bi-directional flow chord diagrams in D3
This is a library/object that enables chord diagrams with flows in both directions using D3.js http://d3js.org/

This is a fork of the excellent work provided in https://github.com/null2/globalmigration

## Usage
Note that not all config directives are well documented, one would have to experiment a bit... Refer to the original repo for more demos and information.
```javascript
var chart = new d3FlowChord().chart(MYDATASTRUCTURE, {
  element: 'ID OF ELEMENT TO BIND THE CHART TO',
  now: YEAR,
  width: WIDTH OF THE CHART,
  HEIGHT: HEIGHT OF THE CHART,
	animationDuration: 500,
	watchKeypress: false,
	margin: 35,
	infoPopupDelay: 500,
	sourcePadding: 0,
	arcPadding: 0.05,
	labelPadding: 10,
	targetPadding: 8,
	layout: {
		threshold: 0,
		labelThreshold: 5,
		outFlowfirst: true,
		colors: n2ndata.colors
	}
});
chart.draw(0, null, MYCALLBACK(OPTIONAL));
}
```
See the original repo on how to format the data structure.

## Changes compared to the original repo
* Fixes for config parameters, when 0 - there was bug that interpreted these as undefined
* Config directive to set inflow/outflow first for each group
* Moved to be a separate object to be instantiated, instead of an object in the window (global) scope
* Code cleanup (cosmetic)
* Callback after draw
* Merged into one file/library

## License
Copyright (c) 2015 Hugo Ahlenius, http://nordpil.com
Copyright (c) 2013 null2 GmbH Berlin  

This work is licensed under a MIT license
