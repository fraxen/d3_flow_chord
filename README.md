# Bi-directional flow chord diagrams in D3
This is a library/object that enables chord diagrams with flows in both directions using D3.js http://d3js.org/

This is a fork of the excellent work provided in https://github.com/null2/globalmigration

## Changes compared to the source
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
