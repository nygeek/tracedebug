# tracedebug

This module provides trace_debug.py which implements the DebugTrace class.

## Description

The debug machinery is implemented using the Python trace hooks,
thus triggering a callout to a trace function on each method entry
and exit.

## Installation

This module should be installed to support the CNC.  Since none of this has
been added to a public Python library, you will need to install it locally
on your machine.  For the purposes of discussion, let's assume that it is
installed at ```~/projects/h/hp35stack/```

```> git clone https://github.com/nygeek/tracedebug.git```

And then install it for the calculator that uses the stack:

```> pip install -e ~/projects/t/tracedebug```

## Known bugs

Using this module creates a global variable in the code that uses it.  This
results in a warning from pylint.  I should figure out how to eliminate this
requirement.

## License

SPDX-License-Identifier: MIT
Copyright (C) 2026 NYGeek LLC

## Authors

Marc Donner (marc.donner@gmail.com)
