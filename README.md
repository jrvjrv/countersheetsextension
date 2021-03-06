Countersheets Extension for Inkscape
====================================

Inkscape extension for the layout of sheets of cards, tiles, or counters
for boardgames.

Since the extension was originally created for wargame counters, the
generated images in this document will be refered to as counters,
except in examples explicitly about making something else (like sheets
of cards). There is very little in the tool that is specific to
counters though, or to board games. It can be used as a
generic templating tool (mail merge).

Main Features
-------------

* Two-sided counters with back of sheets properly mirrored.
* Templates for counters to generate drawn in Inkscape.
* Use Comma Separated Values (CSV) files for describing what counters to make.
* First column in the CSV says how many of each counter to make.
* Several templates can be combined to make up a single counter.
* Automatically make as many sheets needed to fit all counters.
* Replace text strings and bitmap images for each counter.
* Toggle specified parts of counters on or off for each couter.
* Set colors and other attributes of (parts of) counters.
* Any counters can be mixed on the same sheet (even different sizes).
* Registration marks for manual cutting of the sheets.
* Decide exactly where on a sheet to put blocks of counters, for die cutting.
* Export created sheets to PNG or PDF.
* Export individual counters to PNG images.

Installation
------------

You need Inkscape installed (version 0.91, although 0.48 or 0.47 might still work).

Copy countersheet.py, and countersheet.inx to where Inkscape
looks for extensions. On my Mac and Linux computers this is in
.config/inkscape/extensions.  In Windows it will be something like
C:\Program Files\Inkscape\share\extensions.

After you (re)start Inscape you should find "Create Countersheet"
in the "Boardgames" submenu of the "Extensions" menu.

There is an old tutorial also on youtube by Erulisseuiin:
http://www.youtube.com/watch?v=sZ__PwMZp_8
While it is for an older version of the Inkscape Board Game Extensions,
it might still be easier to follow than my short instructions above.

I recommend Google or the Inkscape Guild on BoardGameGeek for help.

Getting Started
---------------

You need a SVG file with template objects open in Inkscape, and
a CSV data file with information about what to generate. Run
the Create Countersheet extension and provide the name of
the data file (the other options in the dialog window you can
ignore for now).

Of course making a SVG file and corresponding CSV can be a bit tricky
at first, since the included documentation isn't very helpful, so I
recommend trying to start with the included examples, as
described below.

Example
-------

Open the file svgtests/input/nato.svg in Inkscape. Run the Create
Countersheet extension. For Data File enter the full name, including
absolute path, of the nato1.csv file in the same directory (eg
C:\your\files\countersheetsextension\svgtests\input\nato1.csv).  Leave
other values at their defaults and run the extension. You should see
two new layers with the fronts and backs of two identical counters.
Experiment with adding rows of values in nato1.csv and re-running the
extension to see what happens (tip: after generating the countersheets,
use the undo function (ctrl-Z) to go back to a blank document between
runs).

License
--------

Copyright (C) 2016 Pelle Nilsson

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.


queryAll method is derived from code included in Inkscape 0.91
(share/extensions/text_merge.py) that has this header:

Copyright (C) 2013 Nicolas Dufour (jazzynico)
Direction code from the Restack extension, by Rob Antonishen

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


Documentation is Copyright 2009-2016 Eric Hanuise and Pelle Nilsson,
available under the Creative Commons Attribution 3.0 License
http://creativecommons.org/licenses/by/3.0/


Included examples in the documentation (the SVG and CSV files) are copyright
Pelle Nilsson and made avilable under the Creative Commons Zero License
(https://creativecommons.org/publicdomain/zero/1.0/) for any use (including
commercial). All images used in the examples are by
KenneyNL (https://kenney.itch.io/) made available under the Creative Commons
Zero License.
